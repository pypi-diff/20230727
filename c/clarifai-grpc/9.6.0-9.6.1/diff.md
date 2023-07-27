# Comparing `tmp/clarifai-grpc-9.6.0.tar.gz` & `tmp/clarifai-grpc-9.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-grpc-9.6.0.tar", last modified: Sat Jul  8 06:39:51 2023, max compression
+gzip compressed data, was "clarifai-grpc-9.6.1.tar", last modified: Thu Jul 27 20:49:53 2023, max compression
```

## Comparing `clarifai-grpc-9.6.0.tar` & `clarifai-grpc-9.6.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.676214 clarifai-grpc-9.6.0/clarifai_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/channel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/clarifai_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12533 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/grpc_json_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/channel/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98821 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   386723 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   242782 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   391049 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   378749 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    53274 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.680214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:39:51.676214 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-08 06:39:51.000000 clarifai-grpc-9.6.0/clarifai_grpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 06:39:51.684214 clarifai-grpc-9.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-08 06:39:42.000000 clarifai-grpc-9.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.240931 clarifai-grpc-9.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-27 20:49:53.240931 clarifai-grpc-9.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.232931 clarifai-grpc-9.6.1/clarifai_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.232931 clarifai-grpc-9.6.1/clarifai_grpc/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/clarifai_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.232931 clarifai-grpc-9.6.1/clarifai_grpc/channel/custom_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/custom_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12533 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/grpc_json_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/channel/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.232931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.236931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100804 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/resources_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   394794 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/resources_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/resources_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   250574 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   409364 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   389254 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.236931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21441 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54246 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_code_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.236931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/extensions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/extensions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/test_proto_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/test_proto_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.236931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.240931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/scope/scope_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/scope/scope_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.240931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/types/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/types/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/types/types_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.240931 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/util/extension_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/util/extension_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/util/extension_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:49:53.232931 clarifai-grpc-9.6.1/clarifai_grpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-27 20:49:53.000000 clarifai-grpc-9.6.1/clarifai_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-27 20:49:53.000000 clarifai-grpc-9.6.1/clarifai_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:49:53.000000 clarifai-grpc-9.6.1/clarifai_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 20:49:53.000000 clarifai-grpc-9.6.1/clarifai_grpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 20:49:53.000000 clarifai-grpc-9.6.1/clarifai_grpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:49:53.240931 clarifai-grpc-9.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-27 20:49:41.000000 clarifai-grpc-9.6.1/setup.py
```

### Comparing `clarifai-grpc-9.6.0/LICENSE` & `clarifai-grpc-9.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/PKG-INFO` & `clarifai-grpc-9.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai-grpc
-Version: 9.6.0
+Version: 9.6.1
 Summary: Clarifai gRPC API Client
 Home-page: https://github.com/Clarifai/clarifai-python-grpc
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-grpc-9.6.0/README.md` & `clarifai-grpc-9.6.1/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/channel/clarifai_channel.py` & `clarifai-grpc-9.6.1/clarifai_grpc/channel/clarifai_channel.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py` & `clarifai-grpc-9.6.1/clarifai_grpc/channel/custom_converters/custom_dict_to_message.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py` & `clarifai-grpc-9.6.1/clarifai_grpc/channel/custom_converters/custom_message_to_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         original's method's return JSON object and keep these fields.
         """
 
         js = super(_CustomPrinter, self)._RegularMessageToJsonObject(message, js)
 
         message_descriptor = message.DESCRIPTOR
         for field in message_descriptor.fields:
-
             if (
                 self._ignore_show_empty
                 and not field.GetOptions().Extensions[extensions_pb2.cl_default_float]
             ):
                 continue
             if not field.GetOptions().Extensions[extensions_pb2.cl_show_if_empty]:
                 continue
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/channel/grpc_json_channel.py` & `clarifai-grpc-9.6.1/clarifai_grpc/channel/grpc_json_channel.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/channel/http_client.py` & `clarifai-grpc-9.6.1/clarifai_grpc/channel/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import typing  # noqa
 
 import requests
 
 from clarifai_grpc.channel.errors import ApiError
 
-CLIENT_VERSION = "9.6.0"
+CLIENT_VERSION = "9.6.1"
 OS_VER = os.sys.platform
 PYTHON_VERSION = ".".join(
     map(
         str,
         [
             os.sys.version_info.major,
             os.sys.version_info.minor,
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/resources_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from clarifai_grpc.grpc.api.utils import matrix_pb2 as proto_dot_clarifai_dot_api_dot_utils_dot_matrix__pb2
 from clarifai_grpc.grpc.auth.util import extension_pb2 as proto_dot_clarifai_dot_auth_dot_util_dot_extension__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"proto/clarifai/api/resources.proto\x12\x0c\x63larifai.api\x1a&proto/clarifai/api/status/status.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/api/utils/matrix.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xe5\x03\n\nAnnotation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x30\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x18\n\x10model_version_id\x18\x10 \x01(\t\x12\"\n\x16\x65mbed_model_version_id\x18\x0e \x01(\tB\x02\x18\x01\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07trusted\x18\n \x01(\x08\x42\x02\x18\x01\x12\x13\n\x0binput_level\x18\x11 \x01(\x08\x12/\n\x0e\x63onsensus_info\x18\x12 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07task_id\x18\x13 \x01(\tJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x9c\x04\n\x03\x41pp\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65\x66\x61ult_language\x18\x03 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ult_workflow_id\x18\x04 \x01(\t\x12\x30\n\x10\x64\x65\x66\x61ult_workflow\x18\x17 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14legal_consent_status\x18\x07 \x01(\r\x12)\n\x08metadata\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x11\n\tsample_ms\x18\x0f \x01(\r\x12,\n\nvisibility\x18\x10 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x14\n\x0c\x64\x61ta_tier_id\x18\x12 \x01(\t\x12\x12\n\nis_starred\x18\x13 \x01(\x08\x12\x12\n\nstar_count\x18\x14 \x01(\x05\x12\r\n\x05notes\x18\x15 \x01(\t\x12\"\n\x05image\x18\x16 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x18\n\x08\x41ppQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x90\x02\n\x0c\x43ollaborator\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12 \n\x04user\x18\x03 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x11\n\tendpoints\x18\x05 \x03(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ndeleted_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x01\n\rCollaboration\x12\x1e\n\x03\x61pp\x18\x01 \x01(\x0b\x32\x11.clarifai.api.App\x12%\n\tapp_owner\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x97\x01\n\x05\x41udio\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\naudio_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.AudioInfo\"b\n\tAudioInfo\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x03 \x01(\x02\x12\x10\n\x08\x62it_rate\x18\x04 \x01(\x05\"w\n\x05Track\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x04 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\x12\x0f\n\x07quality\x18\x05 \x01(\x02J\x04\x08\x03\x10\x04\"h\n\x07\x43luster\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x1f\n\x04hits\x18\x04 \x03(\x0b\x32\x11.clarifai.api.Hit\x12\x12\n\nprojection\x18\x05 \x03(\x02\"M\n\x05\x43olor\x12\x0f\n\x07raw_hex\x18\x01 \x01(\t\x12\x1e\n\x03w3c\x18\x02 \x01(\x0b\x32\x11.clarifai.api.W3C\x12\x13\n\x05value\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\" \n\x03W3C\x12\x0b\n\x03hex\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"/\n\x0cUserAppIDSet\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\"J\n\x0bPatchAction\x12\n\n\x02op\x18\x01 \x01(\t\x12!\n\x19merge_conflict_resolution\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"\xa9\x02\n\x07\x43oncept\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1a\n\x05value\x18\x03 \x01(\x02\x42\x0b\xd5\xb5\x18\x00\x00\x80?\x80\xb5\x18\x01\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x06 \x01(\t\x12\x12\n\ndefinition\x18\x07 \x01(\t\x12\x10\n\x08vocab_id\x18\x08 \x01(\t\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\n \x01(\t\x12\x31\n\rkeypoint_info\x18\x0b \x01(\x0b\x32\x1a.clarifai.api.KeypointInfo\"T\n\x0cKeypointInfo\x12\x16\n\x0ekeypoint_names\x18\x01 \x03(\t\x12,\n\x08skeleton\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.KeypointEdge\"&\n\x0cKeypointEdge\x12\n\n\x02k1\x18\x01 \x01(\r\x12\n\n\x02k2\x18\x02 \x01(\r\"\xa4\x01\n\x0c\x43onceptCount\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12:\n\x12\x63oncept_type_count\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12>\n\x14\x64\x65tail_concept_count\x18\x04 \x01(\x0b\x32 .clarifai.api.DetailConceptCount\"B\n\x10\x43onceptTypeCount\x12\x16\n\x08positive\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08negative\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"\xdf\x01\n\x12\x44\x65tailConceptCount\x12\x31\n\tprocessed\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nto_process\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12.\n\x06\x65rrors\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nprocessing\x18\x04 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\"C\n\x0c\x43onceptQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08language\x18\x02 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x03 \x01(\t\"\xd9\x01\n\x0f\x43onceptRelation\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x0fsubject_concept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\x12-\n\x0eobject_concept\x18\x03 \x01(\x0b\x32\x15.clarifai.api.Concept\x12\x11\n\tpredicate\x18\x04 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x05 \x01(\t\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"y\n\x0eKnowledgeGraph\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x17\n\x0f\x65xamples_app_id\x18\x04 \x01(\t\x12\x1f\n\x17sampled_examples_app_id\x18\x05 \x01(\t\"D\n\x11\x43onceptMappingJob\x12\x1a\n\x12knowledge_graph_id\x18\x01 \x01(\t\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"?\n\x0f\x43onceptLanguage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndefinition\x18\x03 \x01(\t\"\xfa\x04\n\x04\x44\x61ta\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Image\x12\"\n\x05video\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Video\x12\'\n\x08\x63oncepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x03geo\x18\x06 \x01(\x0b\x32\x11.clarifai.api.Geo\x12#\n\x06\x63olors\x18\x07 \x03(\x0b\x32\x13.clarifai.api.Color\x12\'\n\x08\x63lusters\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Cluster\x12+\n\nembeddings\x18\t \x03(\x0b\x32\x17.clarifai.api.Embedding\x12%\n\x07regions\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Region\x12#\n\x06\x66rames\x18\x0c \x03(\x0b\x32\x13.clarifai.api.Frame\x12 \n\x04text\x18\r \x01(\x0b\x32\x12.clarifai.api.Text\x12\"\n\x05\x61udio\x18\x0e \x01(\x0b\x32\x13.clarifai.api.Audio\x12#\n\x06tracks\x18\x0f \x03(\x0b\x32\x13.clarifai.api.Track\x12\x30\n\rtime_segments\x18\x10 \x03(\x0b\x32\x19.clarifai.api.TimeSegment\x12\x1f\n\x04hits\x18\x11 \x03(\x0b\x32\x11.clarifai.api.Hit\x12%\n\x08heatmaps\x18\x12 \x03(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x04\x10\x05J\x04\x08\n\x10\x0b\"\x86\x01\n\x06Region\x12\n\n\x02id\x18\x01 \x01(\t\x12-\n\x0bregion_info\x18\x02 \x01(\x0b\x32\x18.clarifai.api.RegionInfo\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\r\n\x05value\x18\x04 \x01(\x02\x12\x10\n\x08track_id\x18\x05 \x01(\t\"\xae\x02\n\nRegionInfo\x12/\n\x0c\x62ounding_box\x18\x01 \x01(\x0b\x32\x19.clarifai.api.BoundingBox\x12 \n\x04mask\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Mask\x12&\n\x07polygon\x18\x05 \x01(\x0b\x32\x15.clarifai.api.Polygon\x12\"\n\x05point\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Point\x12 \n\x04span\x18\x07 \x01(\x0b\x32\x12.clarifai.api.Span\x12\"\n\x05token\x18\x08 \x01(\x0b\x32\x13.clarifai.api.Token\x12/\n\x12keypoint_locations\x18\t \x03(\x0b\x32\x13.clarifai.api.PointJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"o\n\x0b\x42oundingBox\x12\x15\n\x07top_row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08left_col\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nbottom_row\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tright_col\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"4\n\tFrameInfo\x12\x13\n\x05index\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x12\n\x04time\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"b\n\x05\x46rame\x12+\n\nframe_info\x18\x01 \x01(\x0b\x32\x17.clarifai.api.FrameInfo\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12\n\n\x02id\x18\x03 \x01(\t\"0\n\x04Mask\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x01\x10\x02\".\n\x07Polygon\x12#\n\x06points\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Point\"\xb6\x01\n\x05Point\x12\x11\n\x03row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03\x63ol\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\t\n\x01z\x18\x03 \x01(\x02\x12\x32\n\nvisibility\x18\x04 \x01(\x0e\x32\x1e.clarifai.api.Point.Visibility\"H\n\nVisibility\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0f\n\x0bNOT_VISIBLE\x10\x02\x12\x0f\n\x0bNOT_PRESENT\x10\x03\"J\n\x04Span\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"K\n\x05Token\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"7\n\tEmbedding\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x10\x01\x12\x16\n\x0enum_dimensions\x18\x02 \x01(\r\";\n\x08GeoPoint\x12\x17\n\tlongitude\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08latitude\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\"-\n\x08GeoLimit\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x05value\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\":\n\rGeoBoxedPoint\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\"\x89\x01\n\x03Geo\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\x12)\n\tgeo_limit\x18\x02 \x01(\x0b\x32\x16.clarifai.api.GeoLimit\x12,\n\x07geo_box\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.GeoBoxedPoint\"\x9d\x01\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nimage_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.ImageInfoJ\x04\x08\x03\x10\x04\"N\n\tImageInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x12\n\ncolor_mode\x18\x04 \x01(\t\"O\n\tHostedURL\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\r\n\x05sizes\x18\x03 \x03(\t\x12\x13\n\x0b\x63rossorigin\x18\x04 \x01(\t\"\xde\x01\n\x05Input\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x61taset_ids\x18\x07 \x03(\tJ\x04\x08\x03\x10\x04\"1\n\nInputBatch\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\"\xda\x01\n\nInputCount\x12\x17\n\tprocessed\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_process\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x14\n\x06\x65rrors\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nprocessing\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\treindexed\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_reindex\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1c\n\x0ereindex_errors\x18\x07 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nreindexing\x18\x08 \x01(\rB\x04\x80\xb5\x18\x01\"\xba\x03\n\x07\x44\x61taset\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x41\n\x19\x64\x65\x66\x61ult_annotation_filter\x18\x0c \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\r\n\x05notes\x18\x0b \x01(\t\x12-\n\x07version\x18\r \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x12\n\nis_starred\x18\x0e \x01(\x08\x12\x12\n\nstar_count\x18\x0f \x01(\x05J\x04\x08\x06\x10\x07J\x04\x08\n\x10\x0b\"\xd8\x01\n\x10\x41nnotationFilter\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12*\n\x0csaved_search\x18\x08 \x01(\x0b\x32\x14.clarifai.api.SearchJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"b\n\x0c\x44\x61tasetInput\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xae\x06\n\x0e\x44\x61tasetVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x12\n\ndataset_id\x18\x06 \x01(\t\x12H\n\x18\x61nnotation_filter_config\x18\x0f \x01(\x0b\x32$.clarifai.api.AnnotationFilterConfigH\x00\x12@\n\x14model_predict_config\x18\x12 \x01(\x0b\x32 .clarifai.api.ModelPredictConfigH\x00\x12+\n\x06status\x18\x08 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x43\n\x0fprocessing_info\x18\x13 \x01(\x0b\x32*.clarifai.api.DatasetVersionProcessingInfo\x12:\n\x07metrics\x18\x10 \x03(\x0b\x32).clarifai.api.DatasetVersion.MetricsEntry\x12;\n\x0b\x65xport_info\x18\x11 \x01(\x0b\x32&.clarifai.api.DatasetVersionExportInfo\x12)\n\x08metadata\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x1f\n\x17\x65mbed_model_version_ids\x18\x0e \x03(\t\x1aS\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics:\x02\x38\x01\x42\r\n\x0b\x64\x61ta_configJ\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0c\"p\n\x16\x41nnotationFilterConfig\x12\x39\n\x11\x61nnotation_filter\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x1b\n\x13ignore_empty_inputs\x18\x02 \x01(\x08\"8\n\x12ModelPredictConfig\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Model\"\xc3\x08\n\x15\x44\x61tasetVersionMetrics\x12\x32\n\x0cinputs_count\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12<\n\x16unlabeled_inputs_count\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1ainputs_with_metadata_count\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12;\n\x15inputs_with_geo_count\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x33\n\rregions_count\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12-\n\x16region_location_matrix\x18\x15 \x01(\x0b\x32\r.MatrixUint64\x12:\n\x14\x62ounding_boxes_count\x18\x16 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x34\n\x0epolygons_count\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0cpoints_count\x18\x18 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmasks_count\x18\x19 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_inputs_count\x18< \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_frames_count\x18= \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0c\x66rames_count\x18\x1e \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x12\x66rame_inputs_count\x18\x46 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x36\n\x10\x65mbeddings_count\x18( \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_input_tags_count\x18\x32 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1apositive_region_tags_count\x18\x33 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_frame_tags_count\x18\x34 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"\xca\x01\n\x1a\x44\x61tasetVersionMetricsGroup\x12\x13\n\x0bparent_path\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12%\n\x05value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x34\n\x07metrics\x18\x04 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics\"\xd0\x01\n\x18\x44\x61tasetVersionExportInfo\x12\x42\n\x16\x63larifai_data_protobuf\x18\x01 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12>\n\x12\x63larifai_data_json\x18\x03 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12\x30\n\x04\x63oco\x18\x02 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\"\xb4\x01\n\x14\x44\x61tasetVersionExport\x12\x38\n\x06\x66ormat\x18\x01 \x01(\x0e\x32(.clarifai.api.DatasetVersionExportFormat\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x04\x12\x1a\n\x12include_embeddings\x18\x05 \x01(\x08\"f\n\x1c\x44\x61tasetVersionProcessingInfo\x12\x46\n\x18\x66rame_interpolation_info\x18\x01 \x01(\x0b\x32$.clarifai.api.FrameInterpolationInfo\"+\n\x16\x46rameInterpolationInfo\x12\x11\n\tsample_ms\x18\x01 \x01(\r\"n\n\x19WorkflowResultsSimilarity\x12(\n\x0bprobe_input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12\'\n\x0cpool_results\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Hit\"\xf4\x01\n\x03Key\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x07 \x03(\t\x12\x1f\n\x04\x61pps\x18\x04 \x03(\x0b\x32\x11.clarifai.api.App\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61uthorized_idp_ids\x18\t \x03(\t\"\xd8\x07\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x04name\x18\x02 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x06\x61pp_id\x18\x04 \x01(\tB\x04\x80\xb5\x18\x01\x12\x31\n\x0boutput_info\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfoB\x02\x18\x01\x12\x31\n\rmodel_version\x18\x06 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x18\n\x0c\x64isplay_name\x18\x07 \x01(\tB\x02\x18\x01\x12\x0f\n\x07user_id\x18\t \x01(\t\x12/\n\ninput_info\x18\x0c \x01(\x0b\x32\x17.clarifai.api.InputInfoB\x02\x18\x01\x12/\n\ntrain_info\x18\r \x01(\x0b\x32\x17.clarifai.api.TrainInfoB\x02\x18\x01\x12\x31\n\x11\x64\x65\x66\x61ult_eval_info\x18\x1e \x01(\x0b\x32\x16.clarifai.api.EvalInfo\x12\x15\n\rmodel_type_id\x18\x0e \x01(\t\x12\x0c\n\x04task\x18\x1a \x01(\t\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\x12)\n\x08metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07presets\x18\x1b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05notes\x18\x12 \x01(\t\x12\x16\n\x08toolkits\x18\x14 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tuse_cases\x18\x15 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tlanguages\x18\x19 \x03(\tB\x04\x80\xb5\x18\x01\x12\x33\n\x0elanguages_full\x18\x1f \x03(\x0b\x32\x15.clarifai.api.FullTagB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18  \x03(\tB\x04\x80\xb5\x18\x01\x12\x12\n\nis_starred\x18\x16 \x01(\x08\x12\x12\n\nstar_count\x18\x17 \x01(\x05\x12\x31\n\x0bimport_info\x18\x18 \x01(\x0b\x32\x18.clarifai.api.ImportInfoB\x02\x18\x01\x12\x38\n\x14workflow_recommended\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.BoolValueJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x1c\x10\x1d\"t\n\x0eModelReference\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x97\x01\n\x18ModelVersionInputExample\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"\xd4\x01\n\nOutputInfo\x12 \n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x31\n\routput_config\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12\x0f\n\x07message\x18\x03 \x01(\t\x12+\n\nfields_map\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"a\n\tInputInfo\x12+\n\nfields_map\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\"4\n\tTrainInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"3\n\x08\x45valInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"5\n\nImportInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xdf\x03\n\x0cOutputConfig\x12\'\n\x1b\x63oncepts_mutually_exclusive\x18\x01 \x01(\x08\x42\x02\x18\x01\x12\x1d\n\x11\x65xisting_model_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x1c\n\x10hyper_parameters\x18\x05 \x01(\tB\x02\x18\x01\x12\x1a\n\x0cmax_concepts\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\tmin_value\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12.\n\x0fselect_concepts\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x18\n\x10training_timeout\x18\t \x01(\r\x12\x11\n\tsample_ms\x18\n \x01(\r\x12-\n\x0chyper_params\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x16\x65mbed_model_version_id\x18\x0e \x01(\t\x12)\n!fail_on_missing_positive_examples\x18\x0f \x01(\x08\x12\x33\n\x0emodel_metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x10\x10\x11J\x04\x08\x12\x10\x13\"\xd2\x03\n\tModelType\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cinput_fields\x18\x05 \x03(\t\x12\x15\n\routput_fields\x18\x06 \x03(\t\x12\x11\n\ttrainable\x18\x08 \x01(\x08\x12\x11\n\tcreatable\x18\t \x01(\x08\x12\x15\n\rinternal_only\x18\n \x01(\x08\x12\x37\n\x11model_type_fields\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\"\n\x1arequires_sequential_frames\x18\x0c \x01(\x08\x12;\n\x15\x65xpected_input_layers\x18\x10 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12<\n\x16\x65xpected_output_layers\x18\x11 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12\x35\n\x0f\x65valuation_type\x18\x12 \x01(\x0e\x32\x1c.clarifai.api.EvaluationTypeJ\x04\x08\x07\x10\x08J\x04\x08\x04\x10\x05J\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10\"\x89\x01\n\x0eModelLayerInfo\x12\x17\n\x0f\x64\x61ta_field_name\x18\x01 \x01(\t\x12(\n\x06shapes\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LayerShape\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1f\n\x17requires_label_filename\x18\x04 \x01(\x08\"D\n\x12TritonCondaEnvInfo\x12\x16\n\x0e\x63onda_pack_url\x18\x01 \x01(\t\x12\x16\n\x0e\x63onda_yaml_url\x18\x02 \x01(\t\"l\n\nLayerShape\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x10\n\x08max_dims\x18\x02 \x03(\x05\x12)\n\tdata_type\x18\x03 \x01(\x0e\x32\x16.clarifai.api.DataType\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xd2\x05\n\x0eModelTypeField\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x43\n\nfield_type\x18\x02 \x01(\x0e\x32/.clarifai.api.ModelTypeField.ModelTypeFieldType\x12-\n\rdefault_value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0bplaceholder\x18\x05 \x01(\t\x12\x42\n\x17model_type_enum_options\x18\x06 \x03(\x0b\x32!.clarifai.api.ModelTypeEnumOption\x12\x15\n\rinternal_only\x18\x07 \x01(\x08\x12\x10\n\x08required\x18\x08 \x01(\x08\x12?\n\x15model_type_range_info\x18\t \x01(\x0b\x32 .clarifai.api.ModelTypeRangeInfo\"\xe5\x02\n\x12ModelTypeFieldType\x12!\n\x1dINVALID_MODEL_TYPE_FIELD_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\n\n\x06NUMBER\x10\x03\x12\x15\n\x11\x41RRAY_OF_CONCEPTS\x10\x04\x12$\n ARRAY_OF_CONCEPTS_WITH_THRESHOLD\x10\x05\x12\t\n\x05RANGE\x10\x07\x12\x08\n\x04\x45NUM\x10\x08\x12\x11\n\rCOLLABORATORS\x10\t\x12\x08\n\x04JSON\x10\n\x12\x14\n\x10\x41RRAY_OF_NUMBERS\x10\x0b\x12\x19\n\x15WORKFLOW_EMBED_MODELS\x10\x0c\x12\x14\n\x10\x41RRAY_OF_STRINGS\x10\r\x12\x12\n\x0eRECURSIVE_ENUM\x10\x0e\x12\x0f\n\x0bPYTHON_CODE\x10\x0f\x12\x0e\n\nDATASET_ID\x10\x10\x12\x16\n\x12\x44\x41TASET_VERSION_ID\x10\x11\"\x04\x08\x06\x10\x06\"<\n\x12ModelTypeRangeInfo\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03max\x18\x02 \x01(\x02\x12\x0c\n\x04step\x18\x03 \x01(\x02\"\xd4\x01\n\x13ModelTypeEnumOption\x12\n\n\x02id\x18\x01 \x01(\t\x12\x37\n\x07\x61liases\x18\x05 \x03(\x0b\x32&.clarifai.api.ModelTypeEnumOptionAlias\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x37\n\x11model_type_fields\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\x15\n\rinternal_only\x18\x04 \x01(\x08\x12\x13\n\x0brecommended\x18\x06 \x01(\x08\"C\n\x18ModelTypeEnumOptionAlias\x12\x0e\n\x06id_int\x18\x01 \x01(\x03\x12\x17\n\x0fwildcard_string\x18\x02 \x01(\t\"7\n\nModelQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rmodel_type_id\x18\x03 \x01(\tJ\x04\x08\x02\x10\x03\"\xfc\x05\n\x0cModelVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x04 \x01(\r\x12*\n\x07metrics\x18\x05 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12\x19\n\x11total_input_count\x18\x06 \x01(\r\x12\x44\n\x17pretrained_model_config\x18\x07 \x01(\x0b\x32#.clarifai.api.PretrainedModelConfig\x12\x30\n\x0c\x63ompleted_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\r \x01(\t\x12\x0f\n\x07user_id\x18\x0e \x01(\t\x12/\n\x0bmodified_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07license\x18\x11 \x01(\t\x12-\n\x0boutput_info\x18\x13 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\x12+\n\ninput_info\x18\x14 \x01(\x0b\x32\x17.clarifai.api.InputInfo\x12+\n\ntrain_info\x18\x15 \x01(\x0b\x32\x17.clarifai.api.TrainInfo\x12-\n\x0bimport_info\x18\x16 \x01(\x0b\x32\x18.clarifai.api.ImportInfo\x12\x11\n\ttrain_log\x18\x17 \x01(\tJ\x04\x08\t\x10\nJ\x04\x08\x12\x10\x13\"\xa1\x01\n\x15PretrainedModelConfig\x12\x31\n\x10input_fields_map\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x11output_fields_map\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rmodel_zip_url\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06\">\n\nTrainStats\x12\x30\n\nloss_curve\x18\x01 \x03(\x0b\x32\x1c.clarifai.api.LossCurveEntry\"B\n\x0eLossCurveEntry\x12\r\n\x05\x65poch\x18\x01 \x01(\r\x12\x13\n\x0bglobal_step\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\x02\"1\n\nLabelCount\x12\x14\n\x0c\x63oncept_name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"L\n\x11LabelDistribution\x12\x37\n\x15positive_label_counts\x18\x01 \x03(\x0b\x32\x18.clarifai.api.LabelCount\"B\n\x17\x43ooccurrenceMatrixEntry\x12\x0b\n\x03row\x18\x01 \x01(\t\x12\x0b\n\x03\x63ol\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"`\n\x12\x43ooccurrenceMatrix\x12\x35\n\x06matrix\x18\x01 \x03(\x0b\x32%.clarifai.api.CooccurrenceMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"N\n\x14\x43onfusionMatrixEntry\x12\x11\n\tpredicted\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x02 \x01(\t\x12\x13\n\x05value\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"Z\n\x0f\x43onfusionMatrix\x12\x32\n\x06matrix\x18\x01 \x03(\x0b\x32\".clarifai.api.ConfusionMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"t\n\x03ROC\x12\x11\n\x03\x66pr\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03tpr\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x15\n\rfpr_per_image\x18\x04 \x03(\x02\x12\x16\n\x0e\x66pr_per_object\x18\x05 \x03(\x02\"_\n\x14PrecisionRecallCurve\x12\x14\n\x06recall\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tprecision\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\"\xea\x02\n\rBinaryMetrics\x12\x15\n\x07num_pos\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_neg\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_tot\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x10\n\x02\x66\x31\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12&\n\x07\x63oncept\x18\x06 \x01(\x0b\x32\x15.clarifai.api.Concept\x12$\n\troc_curve\x18\x07 \x01(\x0b\x32\x11.clarifai.api.ROC\x12\x42\n\x16precision_recall_curve\x18\x08 \x01(\x0b\x32\".clarifai.api.PrecisionRecallCurve\x12\x15\n\ravg_precision\x18\t \x01(\x02\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x10\n\x08\x61rea_min\x18\x0b \x01(\x01\x12\x10\n\x08\x61rea_max\x18\x0c \x01(\x01\x12\x0b\n\x03iou\x18\r \x01(\x02\"\x91\x01\n\x0eTrackerMetrics\x12\x10\n\x08mot_mota\x18\x01 \x01(\x02\x12\x18\n\x10mot_num_switches\x18\x02 \x01(\x05\x12\x12\n\nmorse_frag\x18\x03 \x01(\x02\x12\x15\n\ravg_precision\x18\x04 \x01(\x02\x12\x0c\n\x04\x61iid\x18\x05 \x01(\t\x12\x1a\n\x12unique_switch_rate\x18\x06 \x01(\x02\"\xd9\x01\n\x10\x45valTestSetEntry\x12\"\n\x05input\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\x12predicted_concepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x34\n\x15ground_truth_concepts\x18\x04 \x03(\x0b\x32\x15.clarifai.api.Concept\x12,\n\nannotation\x18\x05 \x01(\x0b\x32\x18.clarifai.api.AnnotationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xcd\x01\n\x0eLOPQEvalResult\x12\t\n\x01k\x18\x01 \x01(\x05\x12#\n\x15recall_vs_brute_force\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1akendall_tau_vs_brute_force\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1amost_frequent_code_percent\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tlopq_ndcg\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10\x62rute_force_ndcg\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\"\x8c\x03\n\x0eMetricsSummary\x12\x19\n\rtop1_accuracy\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rtop5_accuracy\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x1f\n\x11macro_avg_roc_auc\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1f\n\x11macro_std_roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_avg_f1_score\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_std_f1_score\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x13macro_avg_precision\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10macro_avg_recall\x18\x08 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x19mean_avg_precision_iou_50\x18\n \x01(\x02\x12$\n\x1cmean_avg_precision_iou_range\x18\x0b \x01(\x02\x12\x32\n\x0clopq_metrics\x18\t \x03(\x0b\x32\x1c.clarifai.api.LOPQEvalResult\"\xd4\x05\n\x0b\x45valMetrics\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\n\n\x02id\x18\n \x01(\t\x12\"\n\x05model\x18\r \x01(\x0b\x32\x13.clarifai.api.Model\x12\x33\n\x14ground_truth_dataset\x18\x0e \x01(\x0b\x32\x15.clarifai.api.Dataset\x12-\n\x07summary\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.MetricsSummary\x12\x37\n\x10\x63onfusion_matrix\x18\x03 \x01(\x0b\x32\x1d.clarifai.api.ConfusionMatrix\x12=\n\x13\x63ooccurrence_matrix\x18\x04 \x01(\x0b\x32 .clarifai.api.CooccurrenceMatrix\x12\x35\n\x0clabel_counts\x18\x05 \x01(\x0b\x32\x1f.clarifai.api.LabelDistribution\x12\x33\n\x0e\x62inary_metrics\x18\x06 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x30\n\x08test_set\x18\x07 \x03(\x0b\x32\x1e.clarifai.api.EvalTestSetEntry\x12\x34\n\x0fmetrics_by_area\x18\x08 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x10metrics_by_class\x18\t \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x0ftracker_metrics\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.TrackerMetrics\x12)\n\teval_info\x18\x0c \x01(\x0b\x32\x16.clarifai.api.EvalInfo\"\xb7\x01\n\x0b\x46ieldsValue\x12\x18\n\x10\x63onfusion_matrix\x18\x01 \x01(\x08\x12\x1b\n\x13\x63ooccurrence_matrix\x18\x02 \x01(\x08\x12\x14\n\x0clabel_counts\x18\x03 \x01(\x08\x12\x16\n\x0e\x62inary_metrics\x18\x04 \x01(\x08\x12\x10\n\x08test_set\x18\x05 \x01(\x08\x12\x17\n\x0fmetrics_by_area\x18\x06 \x01(\x08\x12\x18\n\x10metrics_by_class\x18\x07 \x01(\x08\"\xdb\x01\n\x06Output\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12 \n\x04\x64\x61ta\x18\x06 \x01(\x0b\x32\x12.clarifai.api.Data\"4\n\tScopeDeps\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\":\n\x0c\x45ndpointDeps\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\"\x8d\x01\n\x03Hit\x12\x13\n\x05score\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\x12,\n\nannotation\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\"#\n\x08HitCount\x12\x17\n\x0f\x65stimated_total\x18\x01 \x01(\x04\"\x8d\x01\n\x03\x41nd\x12\"\n\x05input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12$\n\x06output\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Output\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x88\x01\n\x05Query\x12#\n\x04\x61nds\x18\x01 \x03(\x0b\x32\x11.clarifai.api.AndB\x02\x18\x01\x12\x10\n\x08language\x18\x02 \x01(\t\x12%\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Filter\x12!\n\x05ranks\x18\x04 \x03(\x0b\x32\x12.clarifai.api.Rank\"\xd6\x03\n\x06Search\x12\"\n\x05query\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Query\x12\n\n\x02id\x18\x02 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x05\x61s_of\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08git_hash\x18\x06 \x01(\t\x12.\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\talgorithm\x18\t \x01(\t\x12\x0c\n\x04save\x18\n \x01(\x08\x12\x11\n\tmin_value\x18\x0b \x01(\x02\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12+\n\x06metric\x18\r \x01(\x0e\x32\x1b.clarifai.api.Search.Metric\"I\n\x06Metric\x12\x12\n\x0eMETRIC_NOT_SET\x10\x00\x12\x16\n\x12\x45UCLIDEAN_DISTANCE\x10\x01\x12\x13\n\x0f\x43OSINE_DISTANCE\x10\x02\"\xa4\x01\n\x06\x46ilter\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x38\n\x17last_updated_time_range\x18\x06 \x01(\x0b\x32\x17.clarifai.api.TimeRange\"i\n\tTimeRange\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x04Rank\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x8d\x02\n\x17\x41nnotationSearchMetrics\x12*\n\x0cground_truth\x18\x01 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Search\x12*\n\x07metrics\x18\x03 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x05 \x01(\r\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"\x91\x01\n\x04Text\x12\x0b\n\x03raw\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x1b\n\x13\x61llow_duplicate_url\x18\x03 \x01(\x08\x12\'\n\x06hosted\x18\x04 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12)\n\ttext_info\x18\x05 \x01(\x0b\x32\x16.clarifai.api.TextInfo\"0\n\x08TextInfo\x12\x12\n\nchar_count\x18\x01 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x02 \x01(\t\"\xfc\x05\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\rprimary_email\x18\x02 \x01(\tB\x02\x18\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x14\n\x0c\x63ompany_name\x18\x05 \x01(\t\x12\x11\n\tjob_title\x18\x13 \x01(\t\x12\x10\n\x08job_role\x18\x14 \x01(\t\x12\x15\n\tbill_type\x18\x07 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x11\x64\x61te_gdpr_consent\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_tos_consent\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12>\n\x16\x64\x61te_marketing_consent\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_pii_consent\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12-\n\x08metadata\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x37\n\x0f\x65mail_addresses\x18\x0c \x03(\x0b\x32\x1a.clarifai.api.EmailAddressB\x02\x18\x01\x12#\n\x17two_factor_auth_enabled\x18\x0f \x01(\x08\x42\x02\x18\x01\x12\x17\n\x0bteams_count\x18\x10 \x01(\rB\x02\x18\x01\x12\x12\n\nis_starred\x18\x15 \x01(\x08\x12\x12\n\nstar_count\x18\x16 \x01(\x05\x12,\n\nvisibility\x18\x11 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12-\n\x0buser_detail\x18\x12 \x01(\x0b\x32\x18.clarifai.api.UserDetailJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\xd1\x03\n\nUserDetail\x12\x15\n\rprimary_email\x18\x01 \x01(\t\x12\x11\n\tbill_type\x18\x02 \x01(\t\x12\x35\n\x11\x64\x61te_gdpr_consent\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_tos_consent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x64\x61te_marketing_consent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_pii_consent\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x33\n\x0f\x65mail_addresses\x18\x07 \x03(\x0b\x32\x1a.clarifai.api.EmailAddress\x12\x1f\n\x17two_factor_auth_enabled\x18\t \x01(\x08\x12\x13\n\x0bteams_count\x18\n \x01(\r\x12\x0f\n\x07\x63ountry\x18\x0b \x01(\t\x12\r\n\x05state\x18\x0c \x01(\tJ\x04\x08\x08\x10\t\"R\n\x0c\x45mailAddress\x12\x13\n\x05\x65mail\x18\x01 \x01(\tB\x04\x80\xb5\x18\x01\x12\x15\n\x07primary\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08verified\x18\x03 \x01(\x08\x42\x04\x80\xb5\x18\x01\"\x1d\n\x08Password\x12\x11\n\tplaintext\x18\x01 \x01(\t\"\x86\x03\n\x12PasswordViolations\x12\x16\n\x0eminimum_length\x18\x01 \x01(\x08\x12\x16\n\x0emaximum_length\x18\x02 \x01(\x08\x12\x19\n\x11upper_case_needed\x18\x03 \x01(\x08\x12\x19\n\x11lower_case_needed\x18\x04 \x01(\x08\x12\x16\n\x0enumeric_needed\x18\x05 \x01(\x08\x12\x1f\n\x17non_alphanumeric_needed\x18\x06 \x01(\x08\x12\x16\n\x0epassword_reuse\x18\x07 \x01(\x08\x12\x15\n\rexclude_names\x18\x08 \x01(\x08\x12\x15\n\rexclude_email\x18\t \x01(\x08\x12\x1c\n\x14no_confusing_letters\x18\n \x01(\x08\x12\x1b\n\x13no_simple_passwords\x18\x0b \x01(\x08\x12\x18\n\x10no_common_vocabs\x18\x0c \x01(\x08\x12\x1b\n\x13no_overlap_with_old\x18\r \x01(\x08\x12\x19\n\x11password_lifespan\x18\x0e \x01(\x08\"\xae\x01\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\x15\n\rthumbnail_url\x18\x05 \x01(\t\x12\'\n\x06hosted\x18\x06 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nvideo_info\x18\x07 \x01(\x0b\x32\x17.clarifai.api.VideoInfo\"\x8e\x01\n\tVideoInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0b\n\x03\x66ps\x18\x03 \x01(\x02\x12\x14\n\x0cvideo_format\x18\x04 \x01(\t\x12\x10\n\x08\x62it_rate\x18\x05 \x01(\x05\x12\x13\n\x0b\x66rame_count\x18\x06 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x07 \x01(\x02\"\xcf\x03\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x05nodes\x18\x04 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\x07 \x01(\t\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x07version\x18\t \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x12\n\nis_starred\x18\n \x01(\x08\x12\x12\n\nstar_count\x18\x0b \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\r\n\x05notes\x18\r \x01(\t\x12\x17\n\tuse_cases\x18\x0e \x03(\tB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18\x0f \x03(\tB\x04\x80\xb5\x18\x01\"\xde\x02\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x05nodes\x18\x06 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06\x61pp_id\x18\x08 \x01(\t\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07license\x18\x0b \x01(\t\"\xbd\x01\n\x0cWorkflowNode\x12\n\n\x02id\x18\x01 \x01(\t\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\x12,\n\x0bnode_inputs\x18\x03 \x03(\x0b\x32\x17.clarifai.api.NodeInput\x12\x17\n\x0fsuppress_output\x18\x04 \x01(\x08\x12\x36\n\x14output_info_override\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\"\x1c\n\tNodeInput\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x02\n\x0eWorkflowResult\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12%\n\x07outputs\x18\x06 \x03(\x0b\x32\x14.clarifai.api.Output\x12\x17\n\x0fsuppress_output\x18\x07 \x01(\x08\"\x1b\n\rWorkflowState\x12\n\n\x02id\x18\x01 \x01(\t\"\xd8\x02\n\x0e\x41ppDuplication\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nnew_app_id\x18\x02 \x01(\t\x12\x14\n\x0cnew_app_name\x18\x03 \x01(\t\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x66ilter\x18\x07 \x01(\x0b\x32#.clarifai.api.AppDuplicationFilters\x12\x17\n\x0f\x65xisting_app_id\x18\x08 \x01(\t\x12/\n\x08progress\x18\t \x03(\x0b\x32\x1d.clarifai.api.AppCopyProgress\"/\n\x0f\x41ppCopyProgress\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05\"\x8a\x01\n\x15\x41ppDuplicationFilters\x12\x13\n\x0b\x63opy_inputs\x18\x01 \x01(\x08\x12\x15\n\rcopy_concepts\x18\x02 \x01(\x08\x12\x18\n\x10\x63opy_annotations\x18\x03 \x01(\x08\x12\x13\n\x0b\x63opy_models\x18\x04 \x01(\x08\x12\x16\n\x0e\x63opy_workflows\x18\x05 \x01(\x08\"\xfa\x02\n\nLabelOrder\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x61uto_release\x18\x04 \x01(\x08\x12\x17\n\x0f\x61llow_empty_tag\x18\x05 \x01(\x08\x12\x38\n\x14\x64\x65sired_fulfill_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15\x65stimate_fulfill_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x04task\x18\x08 \x01(\x0b\x32\x12.clarifai.api.Task\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb7\x06\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.clarifai.api.Task.TaskType\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12(\n\x06worker\x18\x06 \x01(\x0b\x32\x18.clarifai.api.TaskWorker\x12\x13\n\x0b\x63oncept_ids\x18\x07 \x03(\t\x12\x33\n\x0cinput_source\x18\x08 \x01(\x0b\x32\x1d.clarifai.api.TaskInputSource\x12\x11\n\tsample_ms\x18\t \x01(\r\x12\x33\n\x0c\x61i_assistant\x18\n \x01(\x0b\x32\x1d.clarifai.api.TaskAIAssistant\x12(\n\x06review\x18\x0b \x01(\x0b\x32\x18.clarifai.api.TaskReview\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0c\n\x04name\x18\r \x01(\t\x12:\n\x10\x61i_assist_params\x18\x0e \x01(\x0b\x32 .clarifai.api.AiAssistParameters\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\x0f\n\x07user_id\x18\x11 \x01(\t\x12\x16\n\x0elabel_order_id\x18\x12 \x01(\t\x12+\n\x08\x63oncepts\x18\x13 \x03(\x0b\x32\x19.clarifai.api.TaskConcept\x12#\n\x1b\x64\x65lete_previous_annotations\x18\x14 \x01(\x08\"l\n\x08TaskType\x12\x10\n\x0cTYPE_NOT_SET\x10\x00\x12\x1b\n\x17\x43ONCEPTS_CLASSIFICATION\x10\x01\x12\x1a\n\x16\x42OUNDING_BOX_DETECTION\x10\x02\x12\x15\n\x11POLYGON_DETECTION\x10\x03\"`\n\x12\x41iAssistParameters\x12\x15\n\rmin_threshold\x18\x01 \x01(\x02\x12\x15\n\rmax_threshold\x18\x02 \x01(\x02\x12\x1c\n\x14\x63oncept_relation_ids\x18\x03 \x03(\t\"\x8f\x03\n\nTaskWorker\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskWorker.TaskWorkerStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x04 \x03(\x0b\x32\x12.clarifai.api.User\x12#\n\x06models\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Model\x12)\n\tworkflows\x18\x06 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12T\n\x19partitioned_strategy_info\x18\x03 \x01(\x0b\x32/.clarifai.api.TaskWorkerPartitionedStrategyInfoH\x00\"R\n\x12TaskWorkerStrategy\x12\x1b\n\x17WORKER_STRATEGY_NOT_SET\x10\x00\x12\x0f\n\x0bPARTITIONED\x10\x02\x12\x08\n\x04\x46ULL\x10\x03\"\x04\x08\x01\x10\x01\x42\x0f\n\rstrategy_info\"\xa9\x02\n!TaskWorkerPartitionedStrategyInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.clarifai.api.TaskWorkerPartitionedStrategyInfo.TaskWorkerPartitionedStrategy\x12\x19\n\x11workers_per_input\x18\x02 \x01(\x05\x12(\n\x07weights\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"b\n\x1dTaskWorkerPartitionedStrategy\x12\'\n#PARTITIONED_WORKER_STRATEGY_NOT_SET\x10\x00\x12\n\n\x06\x45VENLY\x10\x01\x12\x0c\n\x08WEIGHTED\x10\x02\"\xc3\x01\n\x0fTaskInputSource\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.clarifai.api.TaskInputSource.TaskInputSourceType\x12\n\n\x02id\x18\x02 \x01(\t\"c\n\x13TaskInputSourceType\x12\x1d\n\x19INPUT_SOURCE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nALL_INPUTS\x10\x01\x12\x10\n\x0cSAVED_SEARCH\x10\x02\x12\x0b\n\x07\x44\x41TASET\x10\x03\"\x90\x03\n\nTaskReview\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskReview.TaskReviewStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x05 \x03(\x0b\x32\x12.clarifai.api.User\x12J\n\x14manual_strategy_info\x18\x03 \x01(\x0b\x32*.clarifai.api.TaskReviewManualStrategyInfoH\x00\x12P\n\x17\x63onsensus_strategy_info\x18\x04 \x01(\x0b\x32-.clarifai.api.TaskReviewConsensusStrategyInfoH\x00\"[\n\x12TaskReviewStrategy\x12 \n\x1cTASK_REVIEW_STRATEGY_NOT_SET\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06MANUAL\x10\x02\x12\r\n\tCONSENSUS\x10\x03\x42\x0f\n\rstrategy_info\"9\n\x1cTaskReviewManualStrategyInfo\x12\x19\n\x11sample_percentage\x18\x01 \x01(\x02\"C\n\x1fTaskReviewConsensusStrategyInfo\x12\x1a\n\x12\x61pproval_threshold\x18\x02 \x01(\rJ\x04\x08\x01\x10\x02\"&\n\x0fTaskAIAssistant\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"\xbc\x01\n\x16TaskStatusCountPerUser\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x15\n\x07pending\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1d\n\x0f\x61waiting_review\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07success\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1b\n\rreview_denied\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\'\n\x19\x61waiting_consensus_review\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\"f\n\x0eThresholdRange\x12\x1a\n\x12is_lower_inclusive\x18\x01 \x01(\x08\x12\x1a\n\x12is_upper_inclusive\x18\x02 \x01(\x08\x12\r\n\x05lower\x18\x03 \x01(\x02\x12\r\n\x05upper\x18\x04 \x01(\x02\"\xad\x01\n\x1fTaskConceptAutoAnnotationConfig\x12\x1d\n\x15\x61nnotation_data_types\x18\x01 \x01(\r\x12\x35\n\x0fthreshold_range\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.ThresholdRange\x12\x34\n\x0bstatus_code\x18\x03 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\"\x84\x01\n\x0bTaskConcept\x12&\n\x07\x63oncept\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Concept\x12M\n\x16\x61uto_annotation_config\x18\x02 \x01(\x0b\x32-.clarifai.api.TaskConceptAutoAnnotationConfig\"\x81\x02\n\tCollector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1d\n\x15pre_queue_workflow_id\x18\x04 \x01(\t\x12\x1e\n\x16post_queue_workflow_id\x18\x05 \x01(\t\x12\x37\n\x10\x63ollector_source\x18\x06 \x01(\x0b\x32\x1d.clarifai.api.CollectorSource\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"t\n\x0f\x43ollectorSource\x12\x61\n\'api_post_model_outputs_collector_source\x18\x02 \x01(\x0b\x32\x30.clarifai.api.APIPostModelOutputsCollectorSource\"\x99\x01\n\"APIPostModelOutputsCollectorSource\x12\x15\n\rmodel_user_id\x18\x01 \x01(\t\x12\x14\n\x0cmodel_app_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x18\n\x10model_version_id\x18\x04 \x01(\t\x12\x1a\n\x12post_inputs_key_id\x18\x05 \x01(\t\"R\n\tStatValue\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04tags\x18\x03 \x03(\t\"\xa6\x01\n\x18StatValueAggregateResult\x12?\n\x15stat_value_aggregates\x18\x01 \x03(\x0b\x32 .clarifai.api.StatValueAggregate\x12I\n\x1astat_value_aggregate_query\x18\x02 \x01(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"t\n\x12StatValueAggregate\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x61ggregate_value\x18\x02 \x01(\x02\x12\r\n\x05\x63ount\x18\x03 \x01(\x04\x12\x0c\n\x04tags\x18\x04 \x03(\t\"\x91\x02\n\x17StatValueAggregateQuery\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x12\n\ntag_groups\x18\x02 \x03(\t\x12;\n\x13stat_value_agg_type\x18\x03 \x01(\x0e\x32\x1e.clarifai.api.StatValueAggType\x12\x39\n\x12stat_time_agg_type\x18\x04 \x01(\x0e\x32\x1d.clarifai.api.StatTimeAggType\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xef\x01\n\x19\x44\x61tasetInputsSearchAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x12\n\ndataset_id\x18\x05 \x01(\t\x12$\n\x06search\x18\x06 \x01(\x0b\x32\x14.clarifai.api.Search\"O\n\x17PCAProjectionComparator\x12\x1a\n\x12\x64istance_threshold\x18\x01 \x01(\x02\x12\x18\n\x10model_version_id\x18\x02 \x01(\t\"K\n\x1b\x44uplicateAnnotationsResults\x12\x16\n\x0e\x64uplicate_cfid\x18\x01 \x03(\t\x12\x14\n\x0cunique_count\x18\x02 \x01(\x05\"\x87\x01\n\nVisibility\x12\x33\n\x08gettable\x18\x01 \x01(\x0e\x32!.clarifai.api.Visibility.Gettable\"D\n\x08Gettable\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\x0b\n\x07PRIVATE\x10\n\x12\x07\n\x03ORG\x10\x1e\x12\n\n\x06PUBLIC\x10\x32\"X\n\x0eTrendingMetric\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\x12\x12\n\nview_count\x18\x04 \x01(\x04\"#\n\x07\x46ullTag\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x0bTimeSegment\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x03 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\"D\n\x08TimeInfo\x12\x12\n\nnum_frames\x18\x01 \x01(\r\x12\x12\n\nbegin_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\"!\n\x0b\x44\x61tasetStar\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\x1f\n\nModuleStar\x12\x11\n\tmodule_id\x18\x01 \x01(\t\"\xe7\x02\n\x06Module\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x07 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x0e\n\x06\x61pp_id\x18\n \x01(\t\x12\x33\n\x0emodule_version\x18\x0b \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x12\n\nis_starred\x18\x0c \x01(\x08\x12\x12\n\nstar_count\x18\r \x01(\x05J\x04\x08\x02\x10\x03\"\xbe\x04\n\rModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\r\n\x05notes\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0egit_commit_url\x18\n \x01(\t\x12\x39\n\nmodule_nav\x18\x0b \x01(\x0b\x32%.clarifai.api.ModuleVersion.ModuleNav\x12\x10\n\x08\x61pproved\x18\x0c \x01(\x08\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x1a\x45\n\x0cModuleSubNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x11\n\tquery_key\x18\x02 \x01(\t\x12\x13\n\x0bquery_value\x18\x03 \x01(\t\x1a]\n\tModuleNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x41\n\x0fmodule_sub_navs\x18\x02 \x03(\x0b\x32(.clarifai.api.ModuleVersion.ModuleSubNavJ\x04\x08\x05\x10\x06\"\xad\x02\n\x16InstalledModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeploy_url\x18\x07 \x01(\t\x12,\n\nvisibility\x18\x08 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06key_id\x18\t \x01(\t\"\xb7\x03\n\rBulkOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\tinput_ids\x18\x02 \x01(\x0b\x32\x16.clarifai.api.InputIDsH\x00\x12&\n\x06search\x18\n \x01(\x0b\x32\x14.clarifai.api.SearchH\x00\x12(\n\x07\x64\x61taset\x18\x0b \x01(\x0b\x32\x15.clarifai.api.DatasetH\x00\x12*\n\toperation\x18\x03 \x01(\x0b\x32\x17.clarifai.api.Operation\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08progress\x18\x06 \x01(\x0b\x32\x16.clarifai.api.Progress\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x0e\n\x0cinput_source\"\x1d\n\x08InputIDs\x12\x11\n\tinput_ids\x18\x01 \x03(\t\"8\n\x08Progress\x12\x11\n\tprocessed\x18\x01 \x01(\r\x12\x19\n\x11last_processed_id\x18\x02 \x01(\t\"\x8a\x04\n\tOperation\x12\x31\n\x0c\x61\x64\x64_concepts\x18\x01 \x01(\x0b\x32\x19.clarifai.api.AddConceptsH\x00\x12\x37\n\x0f\x64\x65lete_concepts\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DeleteConceptsH\x00\x12\x31\n\x0c\x61\x64\x64_metadata\x18\x03 \x01(\x0b\x32\x19.clarifai.api.AddMetadataH\x00\x12\x37\n\x0f\x64\x65lete_metadata\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.DeleteMetadataH\x00\x12\x33\n\roverwrite_geo\x18\x05 \x01(\x0b\x32\x1a.clarifai.api.OverwriteGeoH\x00\x12-\n\ndelete_geo\x18\x06 \x01(\x0b\x32\x17.clarifai.api.DeleteGeoH\x00\x12>\n\x13\x64\x65lete_from_dataset\x18\x07 \x01(\x0b\x32\x1f.clarifai.api.DeleteFromDatasetH\x00\x12\x34\n\x0e\x61\x64\x64_to_dataset\x18\x08 \x01(\x0b\x32\x1a.clarifai.api.AddToDatasetH\x00\x12>\n\x13split_into_datasets\x18\t \x01(\x0b\x32\x1f.clarifai.api.SplitIntoDatasetsH\x00\x42\x0b\n\toperation\"6\n\x0b\x41\x64\x64\x43oncepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\"K\n\x0e\x44\x65leteConcepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x10\n\x08user_ids\x18\x02 \x03(\t\"8\n\x0b\x41\x64\x64Metadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\";\n\x0e\x44\x65leteMetadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\".\n\x0cOverwriteGeo\x12\x1e\n\x03geo\x18\x01 \x01(\x0b\x32\x11.clarifai.api.Geo\"\x0b\n\tDeleteGeo\"\"\n\x0c\x41\x64\x64ToDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\'\n\x11\x44\x65leteFromDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\xcb\x01\n\x11SplitIntoDatasets\x12\x32\n\x0e\x64\x61taset_splits\x18\x01 \x03(\x0b\x32\x1a.clarifai.api.DatasetSplit\x12\x42\n\x06method\x18\x02 \x01(\x0e\x32\x32.clarifai.api.SplitIntoDatasets.DatasetSplitMethod\">\n\x12\x44\x61tasetSplitMethod\x12\x0b\n\x07NOT_SET\x10\x00\x12\x1b\n\x17RANDOM_PERCENTAGE_SPLIT\x10\x01\"[\n\x0c\x44\x61tasetSplit\x12&\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Dataset\x12\x14\n\npercentage\x18\x02 \x01(\rH\x00\x42\r\n\x0bmethod_info\"\xfb\x02\n\x0cInputsAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\x12\x34\n\x08progress\x18\x07 \x01(\x0b\x32\".clarifai.api.InputsAddJobProgress\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x0f\x65xtraction_jobs\x18\n \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\x12%\n\x07uploads\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Upload\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.StatusJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"u\n\x14InputsAddJobProgress\x12\x15\n\rpending_count\x18\x01 \x01(\x04\x12\x19\n\x11in_progress_count\x18\x02 \x01(\x04\x12\x15\n\rsuccess_count\x18\x03 \x01(\x04\x12\x14\n\x0c\x66\x61iled_count\x18\x04 \x01(\x04\"\x95\x02\n\x06Upload\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x63ontent_name\x18\x08 \x01(\t\x12\x16\n\x0e\x63ontent_length\x18\x06 \x01(\x04\x12\x13\n\x0b\x63ontent_url\x18\x07 \x01(\t\"K\n\x11UploadContentPart\x12\x13\n\x0brange_start\x18\x01 \x01(\x04\x12\x13\n\x0bpart_number\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"l\n\x19\x43ustomCodeOperatorRequest\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\x12*\n\x08metadata\x18\xea\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xc8\x02\n\x13InputsExtractionJob\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12;\n\x08progress\x18\x04 \x01(\x0b\x32).clarifai.api.InputsExtractionJobProgress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12M\n\x1cinput_id_conflict_resolution\x18\x07 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"\x97\x02\n\x1bInputsExtractionJobProgress\x12\x1a\n\x12\x61udio_inputs_count\x18\x02 \x01(\x04\x12\x1a\n\x12image_inputs_count\x18\x03 \x01(\x04\x12\x1a\n\x12video_inputs_count\x18\x04 \x01(\x04\x12\x19\n\x11text_inputs_count\x18\x05 \x01(\x04\x12\x1e\n\x16pending_archives_count\x18\x06 \x01(\x04\x12\"\n\x1ain_progress_archives_count\x18\x07 \x01(\x04\x12 \n\x18\x63ompleted_archives_count\x18\x08 \x01(\x04\x12\x1d\n\x15\x66\x61iled_archives_count\x18\t \x01(\x04J\x04\x08\x01\x10\x02\"\xa6\x01\n\x10InputsDataSource\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12(\n\x03url\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.DataSourceURL\x12M\n\x1cinput_id_conflict_resolution\x18\x03 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"V\n\rDataSourceURL\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x38\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32#.clarifai.api.DataSourceCredentials\"\xa7\x01\n\x15\x44\x61taSourceCredentials\x12*\n\x08s3_creds\x18\x01 \x01(\x0b\x32\x16.clarifai.api.AWSCredsH\x00\x12\x13\n\tgcp_creds\x18\x02 \x01(\x0cH\x00\x12\x38\n\x10\x61zure_blob_creds\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.AzureBlobCredsH\x00\x42\r\n\x0b\x63redentialsJ\x04\x08\x03\x10\x04\"K\n\x08\x41WSCreds\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0e\n\x06secret\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\tJ\x04\x08\x01\x10\x02\";\n\x0e\x41zureBlobCreds\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\"\xaf\x01\n\x0cInputsUpload\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x02 \x01(\t\x12$\n\x06upload\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Upload\x12M\n\x1cinput_id_conflict_resolution\x18\x04 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution*\xf9\x01\n\x1e\x44\x61tasetVersionMetricsGroupType\x12.\n*DATASET_VERSION_METRICS_GROUP_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_TYPE\x10\x02\x12\x0e\n\nCONCEPT_ID\x10\n\x12\x12\n\x0e\x43ONCEPTS_COUNT\x10\x0b\x12\x18\n\x14\x42OUNDING_BOXES_COUNT\x10\x14\x12\x12\n\x0ePOLYGONS_COUNT\x10\x15\x12\x10\n\x0cPOINTS_COUNT\x10\x16\x12\x0f\n\x0bMASKS_COUNT\x10\x17\x12\x10\n\x0cPIXELS_COUNT\x10\x1e\x12\x10\n\x0c\x41SPECT_RATIO\x10\x1f*\x85\x01\n\x1a\x44\x61tasetVersionExportFormat\x12)\n%DATASET_VERSION_EXPORT_FORMAT_NOT_SET\x10\x00\x12\x1a\n\x16\x43LARIFAI_DATA_PROTOBUF\x10\x01\x12\x16\n\x12\x43LARIFAI_DATA_JSON\x10\x03\x12\x08\n\x04\x43OCO\x10\x02*H\n\x10\x45xpirationAction\x12\x1d\n\x19\x45XPIRATION_ACTION_NOT_SET\x10\x00\x12\t\n\x05\x44\x45LAY\x10\x01\x12\n\n\x06\x45XPIRY\x10\x02*M\n\x0cLicenseScope\x12\x19\n\x15LICENSE_SCOPE_NOT_SET\x10\x00\x12\x0b\n\x07PREDICT\x10\x01\x12\t\n\x05TRAIN\x10\x02\x12\n\n\x06SEARCH\x10\x03*P\n\x08\x44\x61taType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\t\n\x05UINT8\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04\x46P32\x10\x05*\x8f\x01\n\x0fValueComparator\x12\x1d\n\x19\x43ONCEPT_THRESHOLD_NOT_SET\x10\x00\x12\x10\n\x0cGREATER_THAN\x10\x01\x12\x19\n\x15GREATER_THAN_OR_EQUAL\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x16\n\x12LESS_THAN_OR_EQUAL\x10\x04\x12\t\n\x05\x45QUAL\x10\x05*q\n\x0e\x45valuationType\x12\r\n\tUndefined\x10\x00\x12\x12\n\x0e\x43lassification\x10\x01\x12\r\n\tDetection\x10\x02\x12\x10\n\x0cSegmentation\x10\x03\x12\x0e\n\nClustering\x10\x04\x12\x0b\n\x07Tracker\x10\x05*f\n\x0c\x41PIEventType\x12\x1a\n\x16\x41PI_EVENT_TYPE_NOT_SET\x10\x00\x12\x13\n\x0fON_PREM_PREDICT\x10\x01\x12\x11\n\rON_PREM_TRAIN\x10\x02\x12\x12\n\x0eON_PREM_SEARCH\x10\x03*<\n\x11UsageIntervalType\x12\t\n\x05undef\x10\x00\x12\x07\n\x03\x64\x61y\x10\x01\x12\t\n\x05month\x10\x02\x12\x08\n\x04year\x10\x03*}\n\x12\x41nnotationDataType\x12 \n\x1c\x41NNOTATION_DATA_TYPE_NOT_SET\x10\x00\x12\x07\n\x03TAG\x10\x01\x12\x10\n\x0c\x42OUNDING_BOX\x10\x02\x12\x0b\n\x07POLYGON\x10\x04\x12\t\n\x05POINT\x10\x08\x12\x08\n\x04SPAN\x10\x10\x12\x08\n\x04MASK\x10 *\x1d\n\x08RoleType\x12\x08\n\x04TEAM\x10\x00\x12\x07\n\x03ORG\x10\x01*$\n\x10StatValueAggType\x12\x07\n\x03SUM\x10\x00\x12\x07\n\x03\x41VG\x10\x01*`\n\x0fStatTimeAggType\x12\x0f\n\x0bNO_TIME_AGG\x10\x00\x12\x08\n\x04YEAR\x10\x01\x12\t\n\x05MONTH\x10\x02\x12\x08\n\x04WEEK\x10\x03\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x05\x12\n\n\x06MINUTE\x10\x06*b\n\x13ValidationErrorType\x12!\n\x1dVALIDATION_ERROR_TYPE_NOT_SET\x10\x00\x12\x0e\n\nRESTRICTED\x10\x01\x12\x0c\n\x08\x44\x41TABASE\x10\x02\x12\n\n\x06\x46ORMAT\x10\x03*[\n\x19InputIDConflictResolution\x12(\n$INPUT_ID_CONFLICT_RESOLUTION_NOT_SET\x10\x00\x12\x08\n\x04SKIP\x10\x01\x12\n\n\x06SUFFIX\x10\x02\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"proto/clarifai/api/resources.proto\x12\x0c\x63larifai.api\x1a&proto/clarifai/api/status/status.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/api/utils/matrix.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x82\x04\n\nAnnotation\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x30\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x18\n\x10model_version_id\x18\x10 \x01(\t\x12\"\n\x16\x65mbed_model_version_id\x18\x0e \x01(\tB\x02\x18\x01\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07trusted\x18\n \x01(\x08\x42\x02\x18\x01\x12\x13\n\x0binput_level\x18\x11 \x01(\x08\x12/\n\x0e\x63onsensus_info\x18\x12 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07task_id\x18\x13 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x14 \x01(\tJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x9c\x04\n\x03\x41pp\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65\x66\x61ult_language\x18\x03 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ult_workflow_id\x18\x04 \x01(\t\x12\x30\n\x10\x64\x65\x66\x61ult_workflow\x18\x17 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14legal_consent_status\x18\x07 \x01(\r\x12)\n\x08metadata\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x11\n\tsample_ms\x18\x0f \x01(\r\x12,\n\nvisibility\x18\x10 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x14\n\x0c\x64\x61ta_tier_id\x18\x12 \x01(\t\x12\x12\n\nis_starred\x18\x13 \x01(\x08\x12\x12\n\nstar_count\x18\x14 \x01(\x05\x12\r\n\x05notes\x18\x15 \x01(\t\x12\"\n\x05image\x18\x16 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\r\"\x18\n\x08\x41ppQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x90\x02\n\x0c\x43ollaborator\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12 \n\x04user\x18\x03 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x11\n\tendpoints\x18\x05 \x03(\t\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ndeleted_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa9\x01\n\rCollaboration\x12\x1e\n\x03\x61pp\x18\x01 \x01(\x0b\x32\x11.clarifai.api.App\x12%\n\tapp_owner\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x97\x01\n\x05\x41udio\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\naudio_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.AudioInfo\"b\n\tAudioInfo\x12\x14\n\x0c\x61udio_format\x18\x01 \x01(\t\x12\x13\n\x0bsample_rate\x18\x02 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x03 \x01(\x02\x12\x10\n\x08\x62it_rate\x18\x04 \x01(\x05\"w\n\x05Track\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x04 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\x12\x0f\n\x07quality\x18\x05 \x01(\x02J\x04\x08\x03\x10\x04\"h\n\x07\x43luster\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x1f\n\x04hits\x18\x04 \x03(\x0b\x32\x11.clarifai.api.Hit\x12\x12\n\nprojection\x18\x05 \x03(\x02\"M\n\x05\x43olor\x12\x0f\n\x07raw_hex\x18\x01 \x01(\t\x12\x1e\n\x03w3c\x18\x02 \x01(\x0b\x32\x11.clarifai.api.W3C\x12\x13\n\x05value\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\" \n\x03W3C\x12\x0b\n\x03hex\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"/\n\x0cUserAppIDSet\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\"J\n\x0bPatchAction\x12\n\n\x02op\x18\x01 \x01(\t\x12!\n\x19merge_conflict_resolution\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"\xa9\x02\n\x07\x43oncept\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x1a\n\x05value\x18\x03 \x01(\x02\x42\x0b\xd5\xb5\x18\x00\x00\x80?\x80\xb5\x18\x01\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08language\x18\x05 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x06 \x01(\t\x12\x12\n\ndefinition\x18\x07 \x01(\t\x12\x10\n\x08vocab_id\x18\x08 \x01(\t\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\n \x01(\t\x12\x31\n\rkeypoint_info\x18\x0b \x01(\x0b\x32\x1a.clarifai.api.KeypointInfo\"T\n\x0cKeypointInfo\x12\x16\n\x0ekeypoint_names\x18\x01 \x03(\t\x12,\n\x08skeleton\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.KeypointEdge\"&\n\x0cKeypointEdge\x12\n\n\x02k1\x18\x01 \x01(\r\x12\n\n\x02k2\x18\x02 \x01(\r\"\xa4\x01\n\x0c\x43onceptCount\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12:\n\x12\x63oncept_type_count\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12>\n\x14\x64\x65tail_concept_count\x18\x04 \x01(\x0b\x32 .clarifai.api.DetailConceptCount\"B\n\x10\x43onceptTypeCount\x12\x16\n\x08positive\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08negative\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"\xdf\x01\n\x12\x44\x65tailConceptCount\x12\x31\n\tprocessed\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nto_process\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12.\n\x06\x65rrors\x18\x03 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\x12\x32\n\nprocessing\x18\x04 \x01(\x0b\x32\x1e.clarifai.api.ConceptTypeCount\"C\n\x0c\x43onceptQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08language\x18\x02 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x03 \x01(\t\"\xd9\x01\n\x0f\x43onceptRelation\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x0fsubject_concept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\x12-\n\x0eobject_concept\x18\x03 \x01(\x0b\x32\x15.clarifai.api.Concept\x12\x11\n\tpredicate\x18\x04 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x05 \x01(\t\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"y\n\x0eKnowledgeGraph\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x17\n\x0f\x65xamples_app_id\x18\x04 \x01(\t\x12\x1f\n\x17sampled_examples_app_id\x18\x05 \x01(\t\"D\n\x11\x43onceptMappingJob\x12\x1a\n\x12knowledge_graph_id\x18\x01 \x01(\t\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"?\n\x0f\x43onceptLanguage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndefinition\x18\x03 \x01(\t\"\xfa\x04\n\x04\x44\x61ta\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Image\x12\"\n\x05video\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Video\x12\'\n\x08\x63oncepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1e\n\x03geo\x18\x06 \x01(\x0b\x32\x11.clarifai.api.Geo\x12#\n\x06\x63olors\x18\x07 \x03(\x0b\x32\x13.clarifai.api.Color\x12\'\n\x08\x63lusters\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Cluster\x12+\n\nembeddings\x18\t \x03(\x0b\x32\x17.clarifai.api.Embedding\x12%\n\x07regions\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Region\x12#\n\x06\x66rames\x18\x0c \x03(\x0b\x32\x13.clarifai.api.Frame\x12 \n\x04text\x18\r \x01(\x0b\x32\x12.clarifai.api.Text\x12\"\n\x05\x61udio\x18\x0e \x01(\x0b\x32\x13.clarifai.api.Audio\x12#\n\x06tracks\x18\x0f \x03(\x0b\x32\x13.clarifai.api.Track\x12\x30\n\rtime_segments\x18\x10 \x03(\x0b\x32\x19.clarifai.api.TimeSegment\x12\x1f\n\x04hits\x18\x11 \x03(\x0b\x32\x11.clarifai.api.Hit\x12%\n\x08heatmaps\x18\x12 \x03(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x04\x10\x05J\x04\x08\n\x10\x0b\"\x86\x01\n\x06Region\x12\n\n\x02id\x18\x01 \x01(\t\x12-\n\x0bregion_info\x18\x02 \x01(\x0b\x32\x18.clarifai.api.RegionInfo\x12 \n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x12.clarifai.api.Data\x12\r\n\x05value\x18\x04 \x01(\x02\x12\x10\n\x08track_id\x18\x05 \x01(\t\"\xae\x02\n\nRegionInfo\x12/\n\x0c\x62ounding_box\x18\x01 \x01(\x0b\x32\x19.clarifai.api.BoundingBox\x12 \n\x04mask\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Mask\x12&\n\x07polygon\x18\x05 \x01(\x0b\x32\x15.clarifai.api.Polygon\x12\"\n\x05point\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Point\x12 \n\x04span\x18\x07 \x01(\x0b\x32\x12.clarifai.api.Span\x12\"\n\x05token\x18\x08 \x01(\x0b\x32\x13.clarifai.api.Token\x12/\n\x12keypoint_locations\x18\t \x03(\x0b\x32\x13.clarifai.api.PointJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"o\n\x0b\x42oundingBox\x12\x15\n\x07top_row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08left_col\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nbottom_row\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tright_col\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"4\n\tFrameInfo\x12\x13\n\x05index\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x12\n\x04time\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\"b\n\x05\x46rame\x12+\n\nframe_info\x18\x01 \x01(\x0b\x32\x17.clarifai.api.FrameInfo\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12\n\n\x02id\x18\x03 \x01(\t\"0\n\x04Mask\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ImageJ\x04\x08\x01\x10\x02\".\n\x07Polygon\x12#\n\x06points\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Point\"\xb6\x01\n\x05Point\x12\x11\n\x03row\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03\x63ol\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\t\n\x01z\x18\x03 \x01(\x02\x12\x32\n\nvisibility\x18\x04 \x01(\x0e\x32\x1e.clarifai.api.Point.Visibility\"H\n\nVisibility\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07VISIBLE\x10\x01\x12\x0f\n\x0bNOT_VISIBLE\x10\x02\x12\x0f\n\x0bNOT_PRESENT\x10\x03\"J\n\x04Span\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"K\n\x05Token\x12\x18\n\nchar_start\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x16\n\x08\x63har_end\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x10\n\x08raw_text\x18\x03 \x01(\t\"7\n\tEmbedding\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x10\x01\x12\x16\n\x0enum_dimensions\x18\x02 \x01(\r\";\n\x08GeoPoint\x12\x17\n\tlongitude\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08latitude\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\"-\n\x08GeoLimit\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x05value\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\":\n\rGeoBoxedPoint\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\"\x89\x01\n\x03Geo\x12)\n\tgeo_point\x18\x01 \x01(\x0b\x32\x16.clarifai.api.GeoPoint\x12)\n\tgeo_limit\x18\x02 \x01(\x0b\x32\x16.clarifai.api.GeoLimit\x12,\n\x07geo_box\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.GeoBoxedPoint\"\x9d\x01\n\x05Image\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\'\n\x06hosted\x18\x05 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nimage_info\x18\x06 \x01(\x0b\x32\x17.clarifai.api.ImageInfoJ\x04\x08\x03\x10\x04\"N\n\tImageInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x12\n\ncolor_mode\x18\x04 \x01(\t\"O\n\tHostedURL\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\r\n\x05sizes\x18\x03 \x03(\t\x12\x13\n\x0b\x63rossorigin\x18\x04 \x01(\t\"\xde\x01\n\x05Input\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x61taset_ids\x18\x07 \x03(\tJ\x04\x08\x03\x10\x04\"1\n\nInputBatch\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\"\xda\x01\n\nInputCount\x12\x17\n\tprocessed\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_process\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x14\n\x06\x65rrors\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nprocessing\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\treindexed\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nto_reindex\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1c\n\x0ereindex_errors\x18\x07 \x01(\rB\x04\x80\xb5\x18\x01\x12\x18\n\nreindexing\x18\x08 \x01(\rB\x04\x80\xb5\x18\x01\"\xbe\x04\n\x07\x44\x61taset\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\t \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x41\n\x19\x64\x65\x66\x61ult_annotation_filter\x18\x0c \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12K\n\x17\x64\x65\x66\x61ult_processing_info\x18\x10 \x01(\x0b\x32*.clarifai.api.DatasetVersionProcessingInfo\x12\r\n\x05notes\x18\x0b \x01(\t\x12-\n\x07version\x18\r \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x12\n\nis_starred\x18\x0e \x01(\x08\x12\x12\n\nstar_count\x18\x0f \x01(\x05\x12\x35\n\x0f\x62ookmark_origin\x18\x11 \x01(\x0b\x32\x1c.clarifai.api.BookmarkOriginJ\x04\x08\x06\x10\x07J\x04\x08\n\x10\x0b\"\xd8\x01\n\x10\x41nnotationFilter\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\x12*\n\x0csaved_search\x18\x08 \x01(\x0b\x32\x14.clarifai.api.SearchJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"b\n\x0c\x44\x61tasetInput\x12.\n\ncreated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"\xae\x06\n\x0e\x44\x61tasetVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12\x0f\n\x07user_id\x18\x05 \x01(\t\x12\x12\n\ndataset_id\x18\x06 \x01(\t\x12H\n\x18\x61nnotation_filter_config\x18\x0f \x01(\x0b\x32$.clarifai.api.AnnotationFilterConfigH\x00\x12@\n\x14model_predict_config\x18\x12 \x01(\x0b\x32 .clarifai.api.ModelPredictConfigH\x00\x12+\n\x06status\x18\x08 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x43\n\x0fprocessing_info\x18\x13 \x01(\x0b\x32*.clarifai.api.DatasetVersionProcessingInfo\x12:\n\x07metrics\x18\x10 \x03(\x0b\x32).clarifai.api.DatasetVersion.MetricsEntry\x12;\n\x0b\x65xport_info\x18\x11 \x01(\x0b\x32&.clarifai.api.DatasetVersionExportInfo\x12)\n\x08metadata\x18\x0c \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x1f\n\x17\x65mbed_model_version_ids\x18\x0e \x03(\t\x1aS\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics:\x02\x38\x01\x42\r\n\x0b\x64\x61ta_configJ\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0c\"p\n\x16\x41nnotationFilterConfig\x12\x39\n\x11\x61nnotation_filter\x18\x01 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x1b\n\x13ignore_empty_inputs\x18\x02 \x01(\x08\"8\n\x12ModelPredictConfig\x12\"\n\x05model\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Model\"\xc3\x08\n\x15\x44\x61tasetVersionMetrics\x12\x32\n\x0cinputs_count\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12<\n\x16unlabeled_inputs_count\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1ainputs_with_metadata_count\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12;\n\x15inputs_with_geo_count\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x33\n\rregions_count\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12-\n\x16region_location_matrix\x18\x15 \x01(\x0b\x32\r.MatrixUint64\x12:\n\x14\x62ounding_boxes_count\x18\x16 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x34\n\x0epolygons_count\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0cpoints_count\x18\x18 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0bmasks_count\x18\x19 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_inputs_count\x18< \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x39\n\x13region_frames_count\x18= \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x32\n\x0c\x66rames_count\x18\x1e \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x12\x66rame_inputs_count\x18\x46 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x36\n\x10\x65mbeddings_count\x18( \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_input_tags_count\x18\x32 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12@\n\x1apositive_region_tags_count\x18\x33 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12?\n\x19positive_frame_tags_count\x18\x34 \x01(\x0b\x32\x1c.google.protobuf.UInt64ValueJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"\xca\x01\n\x1a\x44\x61tasetVersionMetricsGroup\x12\x13\n\x0bparent_path\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12%\n\x05value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x34\n\x07metrics\x18\x04 \x01(\x0b\x32#.clarifai.api.DatasetVersionMetrics\"\xd0\x01\n\x18\x44\x61tasetVersionExportInfo\x12\x42\n\x16\x63larifai_data_protobuf\x18\x01 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12>\n\x12\x63larifai_data_json\x18\x03 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\x12\x30\n\x04\x63oco\x18\x02 \x01(\x0b\x32\".clarifai.api.DatasetVersionExport\"\xb4\x01\n\x14\x44\x61tasetVersionExport\x12\x38\n\x06\x66ormat\x18\x01 \x01(\x0e\x32(.clarifai.api.DatasetVersionExportFormat\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x04\x12\x1a\n\x12include_embeddings\x18\x05 \x01(\x08\"f\n\x1c\x44\x61tasetVersionProcessingInfo\x12\x46\n\x18\x66rame_interpolation_info\x18\x01 \x01(\x0b\x32$.clarifai.api.FrameInterpolationInfo\"+\n\x16\x46rameInterpolationInfo\x12\x11\n\tsample_ms\x18\x01 \x01(\r\"n\n\x19WorkflowResultsSimilarity\x12(\n\x0bprobe_input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12\'\n\x0cpool_results\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Hit\"\xf4\x01\n\x03Key\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\x12\x11\n\tendpoints\x18\x07 \x03(\t\x12\x1f\n\x04\x61pps\x18\x04 \x03(\x0b\x32\x11.clarifai.api.App\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12\x61uthorized_idp_ids\x18\t \x03(\t\"\x8f\x08\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x04name\x18\x02 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x06\x61pp_id\x18\x04 \x01(\tB\x04\x80\xb5\x18\x01\x12\x31\n\x0boutput_info\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfoB\x02\x18\x01\x12\x31\n\rmodel_version\x18\x06 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x18\n\x0c\x64isplay_name\x18\x07 \x01(\tB\x02\x18\x01\x12\x0f\n\x07user_id\x18\t \x01(\t\x12/\n\ninput_info\x18\x0c \x01(\x0b\x32\x17.clarifai.api.InputInfoB\x02\x18\x01\x12/\n\ntrain_info\x18\r \x01(\x0b\x32\x17.clarifai.api.TrainInfoB\x02\x18\x01\x12\x31\n\x11\x64\x65\x66\x61ult_eval_info\x18\x1e \x01(\x0b\x32\x16.clarifai.api.EvalInfo\x12\x15\n\rmodel_type_id\x18\x0e \x01(\t\x12\x0c\n\x04task\x18\x1a \x01(\t\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\x12)\n\x08metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\x12(\n\x07presets\x18\x1b \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05notes\x18\x12 \x01(\t\x12\x16\n\x08toolkits\x18\x14 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tuse_cases\x18\x15 \x03(\tB\x04\x80\xb5\x18\x01\x12\x17\n\tlanguages\x18\x19 \x03(\tB\x04\x80\xb5\x18\x01\x12\x33\n\x0elanguages_full\x18\x1f \x03(\x0b\x32\x15.clarifai.api.FullTagB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18  \x03(\tB\x04\x80\xb5\x18\x01\x12\x12\n\nis_starred\x18\x16 \x01(\x08\x12\x12\n\nstar_count\x18\x17 \x01(\x05\x12\x31\n\x0bimport_info\x18\x18 \x01(\x0b\x32\x18.clarifai.api.ImportInfoB\x02\x18\x01\x12\x38\n\x14workflow_recommended\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0f\x62ookmark_origin\x18! \x01(\x0b\x32\x1c.clarifai.api.BookmarkOriginJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x1c\x10\x1d\"t\n\x0eModelReference\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x97\x01\n\x18ModelVersionInputExample\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"\xd4\x01\n\nOutputInfo\x12 \n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x31\n\routput_config\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12\x0f\n\x07message\x18\x03 \x01(\t\x12+\n\nfields_map\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\x90\x01\n\tInputInfo\x12+\n\nfields_map\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\'\n\x06params\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12-\n\x10\x62\x61se_embed_model\x18\x03 \x01(\x0b\x32\x13.clarifai.api.Model\"4\n\tTrainInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"3\n\x08\x45valInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"5\n\nImportInfo\x12\'\n\x06params\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xe3\x03\n\x0cOutputConfig\x12\'\n\x1b\x63oncepts_mutually_exclusive\x18\x01 \x01(\x08\x42\x02\x18\x01\x12\x1d\n\x11\x65xisting_model_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x1c\n\x10hyper_parameters\x18\x05 \x01(\tB\x02\x18\x01\x12\x1a\n\x0cmax_concepts\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\x12\x17\n\tmin_value\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12.\n\x0fselect_concepts\x18\x08 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x18\n\x10training_timeout\x18\t \x01(\r\x12\x11\n\tsample_ms\x18\n \x01(\r\x12-\n\x0chyper_params\x18\r \x01(\x0b\x32\x17.google.protobuf.Struct\x12\"\n\x16\x65mbed_model_version_id\x18\x0e \x01(\tB\x02\x18\x01\x12)\n!fail_on_missing_positive_examples\x18\x0f \x01(\x08\x12\x33\n\x0emodel_metadata\x18\x11 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x10\x10\x11J\x04\x08\x12\x10\x13\"\xd2\x03\n\tModelType\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cinput_fields\x18\x05 \x03(\t\x12\x15\n\routput_fields\x18\x06 \x03(\t\x12\x11\n\ttrainable\x18\x08 \x01(\x08\x12\x11\n\tcreatable\x18\t \x01(\x08\x12\x15\n\rinternal_only\x18\n \x01(\x08\x12\x37\n\x11model_type_fields\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\"\n\x1arequires_sequential_frames\x18\x0c \x01(\x08\x12;\n\x15\x65xpected_input_layers\x18\x10 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12<\n\x16\x65xpected_output_layers\x18\x11 \x03(\x0b\x32\x1c.clarifai.api.ModelLayerInfo\x12\x35\n\x0f\x65valuation_type\x18\x12 \x01(\x0e\x32\x1c.clarifai.api.EvaluationTypeJ\x04\x08\x07\x10\x08J\x04\x08\x04\x10\x05J\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10\"\x89\x01\n\x0eModelLayerInfo\x12\x17\n\x0f\x64\x61ta_field_name\x18\x01 \x01(\t\x12(\n\x06shapes\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LayerShape\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1f\n\x17requires_label_filename\x18\x04 \x01(\x08\"D\n\x12TritonCondaEnvInfo\x12\x16\n\x0e\x63onda_pack_url\x18\x01 \x01(\t\x12\x16\n\x0e\x63onda_yaml_url\x18\x02 \x01(\t\"l\n\nLayerShape\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x10\n\x08max_dims\x18\x02 \x03(\x05\x12)\n\tdata_type\x18\x03 \x01(\x0e\x32\x16.clarifai.api.DataType\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xef\x05\n\x0eModelTypeField\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x43\n\nfield_type\x18\x02 \x01(\x0e\x32/.clarifai.api.ModelTypeField.ModelTypeFieldType\x12-\n\rdefault_value\x18\x03 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x13\n\x0bplaceholder\x18\x05 \x01(\t\x12\x42\n\x17model_type_enum_options\x18\x06 \x03(\x0b\x32!.clarifai.api.ModelTypeEnumOption\x12\x15\n\rinternal_only\x18\x07 \x01(\x08\x12\x10\n\x08required\x18\x08 \x01(\x08\x12?\n\x15model_type_range_info\x18\t \x01(\x0b\x32 .clarifai.api.ModelTypeRangeInfo\"\x82\x03\n\x12ModelTypeFieldType\x12!\n\x1dINVALID_MODEL_TYPE_FIELD_TYPE\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\n\n\x06STRING\x10\x02\x12\n\n\x06NUMBER\x10\x03\x12\x15\n\x11\x41RRAY_OF_CONCEPTS\x10\x04\x12$\n ARRAY_OF_CONCEPTS_WITH_THRESHOLD\x10\x05\x12\t\n\x05RANGE\x10\x07\x12\x08\n\x04\x45NUM\x10\x08\x12\x11\n\rCOLLABORATORS\x10\t\x12\x08\n\x04JSON\x10\n\x12\x14\n\x10\x41RRAY_OF_NUMBERS\x10\x0b\x12\x19\n\x15WORKFLOW_EMBED_MODELS\x10\x0c\x12\x14\n\x10\x41RRAY_OF_STRINGS\x10\r\x12\x12\n\x0eRECURSIVE_ENUM\x10\x0e\x12\x0f\n\x0bPYTHON_CODE\x10\x0f\x12\x0e\n\nDATASET_ID\x10\x10\x12\x16\n\x12\x44\x41TASET_VERSION_ID\x10\x11\x12\x1b\n\x17\x41RRAY_OF_MODEL_CONCEPTS\x10\x12\"\x04\x08\x06\x10\x06\"<\n\x12ModelTypeRangeInfo\x12\x0b\n\x03min\x18\x01 \x01(\x02\x12\x0b\n\x03max\x18\x02 \x01(\x02\x12\x0c\n\x04step\x18\x03 \x01(\x02\"\xd4\x01\n\x13ModelTypeEnumOption\x12\n\n\x02id\x18\x01 \x01(\t\x12\x37\n\x07\x61liases\x18\x05 \x03(\x0b\x32&.clarifai.api.ModelTypeEnumOptionAlias\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x37\n\x11model_type_fields\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12\x15\n\rinternal_only\x18\x04 \x01(\x08\x12\x13\n\x0brecommended\x18\x06 \x01(\x08\"C\n\x18ModelTypeEnumOptionAlias\x12\x0e\n\x06id_int\x18\x01 \x01(\x03\x12\x17\n\x0fwildcard_string\x18\x02 \x01(\t\"7\n\nModelQuery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rmodel_type_id\x18\x03 \x01(\tJ\x04\x08\x02\x10\x03\"\xfc\x05\n\x0cModelVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x04 \x01(\r\x12*\n\x07metrics\x18\x05 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12\x19\n\x11total_input_count\x18\x06 \x01(\r\x12\x44\n\x17pretrained_model_config\x18\x07 \x01(\x0b\x32#.clarifai.api.PretrainedModelConfig\x12\x30\n\x0c\x63ompleted_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\r \x01(\t\x12\x0f\n\x07user_id\x18\x0e \x01(\t\x12/\n\x0bmodified_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07license\x18\x11 \x01(\t\x12-\n\x0boutput_info\x18\x13 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\x12+\n\ninput_info\x18\x14 \x01(\x0b\x32\x17.clarifai.api.InputInfo\x12+\n\ntrain_info\x18\x15 \x01(\x0b\x32\x17.clarifai.api.TrainInfo\x12-\n\x0bimport_info\x18\x16 \x01(\x0b\x32\x18.clarifai.api.ImportInfo\x12\x11\n\ttrain_log\x18\x17 \x01(\tJ\x04\x08\t\x10\nJ\x04\x08\x12\x10\x13\"\xa1\x01\n\x15PretrainedModelConfig\x12\x31\n\x10input_fields_map\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x32\n\x11output_fields_map\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rmodel_zip_url\x18\x06 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06\">\n\nTrainStats\x12\x30\n\nloss_curve\x18\x01 \x03(\x0b\x32\x1c.clarifai.api.LossCurveEntry\"B\n\x0eLossCurveEntry\x12\r\n\x05\x65poch\x18\x01 \x01(\r\x12\x13\n\x0bglobal_step\x18\x02 \x01(\r\x12\x0c\n\x04\x63ost\x18\x03 \x01(\x02\"1\n\nLabelCount\x12\x14\n\x0c\x63oncept_name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\r\"L\n\x11LabelDistribution\x12\x37\n\x15positive_label_counts\x18\x01 \x03(\x0b\x32\x18.clarifai.api.LabelCount\"B\n\x17\x43ooccurrenceMatrixEntry\x12\x0b\n\x03row\x18\x01 \x01(\t\x12\x0b\n\x03\x63ol\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\r\"`\n\x12\x43ooccurrenceMatrix\x12\x35\n\x06matrix\x18\x01 \x03(\x0b\x32%.clarifai.api.CooccurrenceMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"N\n\x14\x43onfusionMatrixEntry\x12\x11\n\tpredicted\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x02 \x01(\t\x12\x13\n\x05value\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\"Z\n\x0f\x43onfusionMatrix\x12\x32\n\x06matrix\x18\x01 \x03(\x0b\x32\".clarifai.api.ConfusionMatrixEntry\x12\x13\n\x0b\x63oncept_ids\x18\x02 \x03(\t\"t\n\x03ROC\x12\x11\n\x03\x66pr\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x11\n\x03tpr\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x15\n\rfpr_per_image\x18\x04 \x03(\x02\x12\x16\n\x0e\x66pr_per_object\x18\x05 \x03(\x02\"_\n\x14PrecisionRecallCurve\x12\x14\n\x06recall\x18\x01 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tprecision\x18\x02 \x03(\x02\x42\x04\x80\xb5\x18\x01\x12\x18\n\nthresholds\x18\x03 \x03(\x02\x42\x04\x80\xb5\x18\x01\"\xea\x02\n\rBinaryMetrics\x12\x15\n\x07num_pos\x18\x01 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_neg\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07num_tot\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x10\n\x02\x66\x31\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12&\n\x07\x63oncept\x18\x06 \x01(\x0b\x32\x15.clarifai.api.Concept\x12$\n\troc_curve\x18\x07 \x01(\x0b\x32\x11.clarifai.api.ROC\x12\x42\n\x16precision_recall_curve\x18\x08 \x01(\x0b\x32\".clarifai.api.PrecisionRecallCurve\x12\x15\n\ravg_precision\x18\t \x01(\x02\x12\x11\n\tarea_name\x18\n \x01(\t\x12\x10\n\x08\x61rea_min\x18\x0b \x01(\x01\x12\x10\n\x08\x61rea_max\x18\x0c \x01(\x01\x12\x0b\n\x03iou\x18\r \x01(\x02\"\x91\x01\n\x0eTrackerMetrics\x12\x10\n\x08mot_mota\x18\x01 \x01(\x02\x12\x18\n\x10mot_num_switches\x18\x02 \x01(\x05\x12\x12\n\nmorse_frag\x18\x03 \x01(\x02\x12\x15\n\ravg_precision\x18\x04 \x01(\x02\x12\x0c\n\x04\x61iid\x18\x05 \x01(\t\x12\x1a\n\x12unique_switch_rate\x18\x06 \x01(\x02\"\xd9\x01\n\x10\x45valTestSetEntry\x12\"\n\x05input\x18\x06 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\x12predicted_concepts\x18\x03 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x34\n\x15ground_truth_concepts\x18\x04 \x03(\x0b\x32\x15.clarifai.api.Concept\x12,\n\nannotation\x18\x05 \x01(\x0b\x32\x18.clarifai.api.AnnotationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xcd\x01\n\x0eLOPQEvalResult\x12\t\n\x01k\x18\x01 \x01(\x05\x12#\n\x15recall_vs_brute_force\x18\x02 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1akendall_tau_vs_brute_force\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12(\n\x1amost_frequent_code_percent\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x17\n\tlopq_ndcg\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10\x62rute_force_ndcg\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\"\x8c\x03\n\x0eMetricsSummary\x12\x19\n\rtop1_accuracy\x18\x01 \x01(\x02\x42\x02\x18\x01\x12\x19\n\rtop5_accuracy\x18\x02 \x01(\x02\x42\x02\x18\x01\x12\x1f\n\x11macro_avg_roc_auc\x18\x03 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1f\n\x11macro_std_roc_auc\x18\x04 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_avg_f1_score\x18\x05 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12 \n\x12macro_std_f1_score\x18\x06 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x13macro_avg_precision\x18\x07 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\x1e\n\x10macro_avg_recall\x18\x08 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12!\n\x19mean_avg_precision_iou_50\x18\n \x01(\x02\x12$\n\x1cmean_avg_precision_iou_range\x18\x0b \x01(\x02\x12\x32\n\x0clopq_metrics\x18\t \x03(\x0b\x32\x1c.clarifai.api.LOPQEvalResult\"\xd4\x05\n\x0b\x45valMetrics\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0f\n\x07user_id\x18\x0f \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\n\n\x02id\x18\n \x01(\t\x12\"\n\x05model\x18\r \x01(\x0b\x32\x13.clarifai.api.Model\x12\x33\n\x14ground_truth_dataset\x18\x0e \x01(\x0b\x32\x15.clarifai.api.Dataset\x12-\n\x07summary\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.MetricsSummary\x12\x37\n\x10\x63onfusion_matrix\x18\x03 \x01(\x0b\x32\x1d.clarifai.api.ConfusionMatrix\x12=\n\x13\x63ooccurrence_matrix\x18\x04 \x01(\x0b\x32 .clarifai.api.CooccurrenceMatrix\x12\x35\n\x0clabel_counts\x18\x05 \x01(\x0b\x32\x1f.clarifai.api.LabelDistribution\x12\x33\n\x0e\x62inary_metrics\x18\x06 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x30\n\x08test_set\x18\x07 \x03(\x0b\x32\x1e.clarifai.api.EvalTestSetEntry\x12\x34\n\x0fmetrics_by_area\x18\x08 \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x10metrics_by_class\x18\t \x03(\x0b\x32\x1b.clarifai.api.BinaryMetrics\x12\x35\n\x0ftracker_metrics\x18\x0b \x03(\x0b\x32\x1c.clarifai.api.TrackerMetrics\x12)\n\teval_info\x18\x0c \x01(\x0b\x32\x16.clarifai.api.EvalInfo\"\xb7\x01\n\x0b\x46ieldsValue\x12\x18\n\x10\x63onfusion_matrix\x18\x01 \x01(\x08\x12\x1b\n\x13\x63ooccurrence_matrix\x18\x02 \x01(\x08\x12\x14\n\x0clabel_counts\x18\x03 \x01(\x08\x12\x16\n\x0e\x62inary_metrics\x18\x04 \x01(\x08\x12\x10\n\x08test_set\x18\x05 \x01(\x08\x12\x17\n\x0fmetrics_by_area\x18\x06 \x01(\x08\x12\x18\n\x10metrics_by_class\x18\x07 \x01(\x08\"\xdb\x01\n\x06Output\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12 \n\x04\x64\x61ta\x18\x06 \x01(\x0b\x32\x12.clarifai.api.Data\"4\n\tScopeDeps\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\":\n\x0c\x45ndpointDeps\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x18\n\x10\x64\x65pending_scopes\x18\x02 \x03(\t\"\x8d\x01\n\x03Hit\x12\x13\n\x05score\x18\x01 \x01(\x02\x42\x04\x80\xb5\x18\x01\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\x12,\n\nannotation\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x05 \x01(\t\"#\n\x08HitCount\x12\x17\n\x0f\x65stimated_total\x18\x01 \x01(\x04\"\x8d\x01\n\x03\x41nd\x12\"\n\x05input\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Input\x12$\n\x06output\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Output\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x88\x01\n\x05Query\x12#\n\x04\x61nds\x18\x01 \x03(\x0b\x32\x11.clarifai.api.AndB\x02\x18\x01\x12\x10\n\x08language\x18\x02 \x01(\t\x12%\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Filter\x12!\n\x05ranks\x18\x04 \x03(\x0b\x32\x12.clarifai.api.Rank\"\xd6\x03\n\x06Search\x12\"\n\x05query\x18\x01 \x01(\x0b\x32\x13.clarifai.api.Query\x12\n\n\x02id\x18\x02 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\x05\x61s_of\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08git_hash\x18\x06 \x01(\t\x12.\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\talgorithm\x18\t \x01(\t\x12\x0c\n\x04save\x18\n \x01(\x08\x12\x11\n\tmin_value\x18\x0b \x01(\x02\x12,\n\nvisibility\x18\x0c \x01(\x0b\x32\x18.clarifai.api.Visibility\x12+\n\x06metric\x18\r \x01(\x0e\x32\x1b.clarifai.api.Search.Metric\"I\n\x06Metric\x12\x12\n\x0eMETRIC_NOT_SET\x10\x00\x12\x16\n\x12\x45UCLIDEAN_DISTANCE\x10\x01\x12\x13\n\x0f\x43OSINE_DISTANCE\x10\x02\"\xa4\x01\n\x06\x46ilter\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12\x38\n\x17last_updated_time_range\x18\x06 \x01(\x0b\x32\x17.clarifai.api.TimeRange\"i\n\tTimeRange\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x04Rank\x12\x0e\n\x06negate\x18\x03 \x01(\x08\x12,\n\nannotation\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Annotation\"\x8d\x02\n\x17\x41nnotationSearchMetrics\x12*\n\x0cground_truth\x18\x01 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Search\x12*\n\x07metrics\x18\x03 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\x12 \n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x1c\n\x14\x61\x63tive_concept_count\x18\x05 \x01(\r\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\"\x91\x01\n\x04Text\x12\x0b\n\x03raw\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x1b\n\x13\x61llow_duplicate_url\x18\x03 \x01(\x08\x12\'\n\x06hosted\x18\x04 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12)\n\ttext_info\x18\x05 \x01(\x0b\x32\x16.clarifai.api.TextInfo\"0\n\x08TextInfo\x12\x12\n\nchar_count\x18\x01 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x02 \x01(\t\"\xfc\x05\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x19\n\rprimary_email\x18\x02 \x01(\tB\x02\x18\x01\x12\x12\n\nfirst_name\x18\x03 \x01(\t\x12\x11\n\tlast_name\x18\x04 \x01(\t\x12\x14\n\x0c\x63ompany_name\x18\x05 \x01(\t\x12\x11\n\tjob_title\x18\x13 \x01(\t\x12\x10\n\x08job_role\x18\x14 \x01(\t\x12\x15\n\tbill_type\x18\x07 \x01(\tB\x02\x18\x01\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x11\x64\x61te_gdpr_consent\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_tos_consent\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12>\n\x16\x64\x61te_marketing_consent\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x38\n\x10\x64\x61te_pii_consent\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12-\n\x08metadata\x18\x0b \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x37\n\x0f\x65mail_addresses\x18\x0c \x03(\x0b\x32\x1a.clarifai.api.EmailAddressB\x02\x18\x01\x12#\n\x17two_factor_auth_enabled\x18\x0f \x01(\x08\x42\x02\x18\x01\x12\x17\n\x0bteams_count\x18\x10 \x01(\rB\x02\x18\x01\x12\x12\n\nis_starred\x18\x15 \x01(\x08\x12\x12\n\nstar_count\x18\x16 \x01(\x05\x12,\n\nvisibility\x18\x11 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12-\n\x0buser_detail\x18\x12 \x01(\x0b\x32\x18.clarifai.api.UserDetailJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\xd1\x03\n\nUserDetail\x12\x15\n\rprimary_email\x18\x01 \x01(\t\x12\x11\n\tbill_type\x18\x02 \x01(\t\x12\x35\n\x11\x64\x61te_gdpr_consent\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_tos_consent\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x64\x61te_marketing_consent\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x64\x61te_pii_consent\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x33\n\x0f\x65mail_addresses\x18\x07 \x03(\x0b\x32\x1a.clarifai.api.EmailAddress\x12\x1f\n\x17two_factor_auth_enabled\x18\t \x01(\x08\x12\x13\n\x0bteams_count\x18\n \x01(\r\x12\x0f\n\x07\x63ountry\x18\x0b \x01(\t\x12\r\n\x05state\x18\x0c \x01(\tJ\x04\x08\x08\x10\t\"R\n\x0c\x45mailAddress\x12\x13\n\x05\x65mail\x18\x01 \x01(\tB\x04\x80\xb5\x18\x01\x12\x15\n\x07primary\x18\x02 \x01(\x08\x42\x04\x80\xb5\x18\x01\x12\x16\n\x08verified\x18\x03 \x01(\x08\x42\x04\x80\xb5\x18\x01\"\x1d\n\x08Password\x12\x11\n\tplaintext\x18\x01 \x01(\t\"\x86\x03\n\x12PasswordViolations\x12\x16\n\x0eminimum_length\x18\x01 \x01(\x08\x12\x16\n\x0emaximum_length\x18\x02 \x01(\x08\x12\x19\n\x11upper_case_needed\x18\x03 \x01(\x08\x12\x19\n\x11lower_case_needed\x18\x04 \x01(\x08\x12\x16\n\x0enumeric_needed\x18\x05 \x01(\x08\x12\x1f\n\x17non_alphanumeric_needed\x18\x06 \x01(\x08\x12\x16\n\x0epassword_reuse\x18\x07 \x01(\x08\x12\x15\n\rexclude_names\x18\x08 \x01(\x08\x12\x15\n\rexclude_email\x18\t \x01(\x08\x12\x1c\n\x14no_confusing_letters\x18\n \x01(\x08\x12\x1b\n\x13no_simple_passwords\x18\x0b \x01(\x08\x12\x18\n\x10no_common_vocabs\x18\x0c \x01(\x08\x12\x1b\n\x13no_overlap_with_old\x18\r \x01(\x08\x12\x19\n\x11password_lifespan\x18\x0e \x01(\x08\"\xae\x01\n\x05Video\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0e\n\x06\x62\x61se64\x18\x02 \x01(\x0c\x12\x1b\n\x13\x61llow_duplicate_url\x18\x04 \x01(\x08\x12\x15\n\rthumbnail_url\x18\x05 \x01(\t\x12\'\n\x06hosted\x18\x06 \x01(\x0b\x32\x17.clarifai.api.HostedURL\x12+\n\nvideo_info\x18\x07 \x01(\x0b\x32\x17.clarifai.api.VideoInfo\"\x8e\x01\n\tVideoInfo\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x0b\n\x03\x66ps\x18\x03 \x01(\x02\x12\x14\n\x0cvideo_format\x18\x04 \x01(\t\x12\x10\n\x08\x62it_rate\x18\x05 \x01(\x05\x12\x13\n\x0b\x66rame_count\x18\x06 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x07 \x01(\x02\"\x86\x04\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x05nodes\x18\x04 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\nvisibility\x18\x06 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0f\n\x07user_id\x18\x07 \x01(\t\x12/\n\x0bmodified_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x07version\x18\t \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x12\n\nis_starred\x18\n \x01(\x08\x12\x12\n\nstar_count\x18\x0b \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\r\n\x05notes\x18\r \x01(\t\x12\x17\n\tuse_cases\x18\x0e \x03(\tB\x04\x80\xb5\x18\x01\x12\x1c\n\x0e\x63heck_consents\x18\x0f \x03(\tB\x04\x80\xb5\x18\x01\x12\x35\n\x0f\x62ookmark_origin\x18\x10 \x01(\x0b\x32\x1c.clarifai.api.BookmarkOrigin\"\xde\x02\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x05 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x05nodes\x18\x06 \x03(\x0b\x32\x1a.clarifai.api.WorkflowNode\x12)\n\x08metadata\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0e\n\x06\x61pp_id\x18\x08 \x01(\t\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07license\x18\x0b \x01(\t\"\xbd\x01\n\x0cWorkflowNode\x12\n\n\x02id\x18\x01 \x01(\t\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\x12,\n\x0bnode_inputs\x18\x03 \x03(\x0b\x32\x17.clarifai.api.NodeInput\x12\x17\n\x0fsuppress_output\x18\x04 \x01(\x08\x12\x36\n\x14output_info_override\x18\x05 \x01(\x0b\x32\x18.clarifai.api.OutputInfo\"\x1c\n\tNodeInput\x12\x0f\n\x07node_id\x18\x01 \x01(\t\"\x81\x02\n\x0eWorkflowResult\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x05model\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Model\x12\"\n\x05input\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Input\x12%\n\x07outputs\x18\x06 \x03(\x0b\x32\x14.clarifai.api.Output\x12\x17\n\x0fsuppress_output\x18\x07 \x01(\x08\"\x1b\n\rWorkflowState\x12\n\n\x02id\x18\x01 \x01(\t\"\xd8\x02\n\x0e\x41ppDuplication\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nnew_app_id\x18\x02 \x01(\t\x12\x14\n\x0cnew_app_name\x18\x03 \x01(\t\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x66ilter\x18\x07 \x01(\x0b\x32#.clarifai.api.AppDuplicationFilters\x12\x17\n\x0f\x65xisting_app_id\x18\x08 \x01(\t\x12/\n\x08progress\x18\t \x03(\x0b\x32\x1d.clarifai.api.AppCopyProgress\"/\n\x0f\x41ppCopyProgress\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05\"\x8a\x01\n\x15\x41ppDuplicationFilters\x12\x13\n\x0b\x63opy_inputs\x18\x01 \x01(\x08\x12\x15\n\rcopy_concepts\x18\x02 \x01(\x08\x12\x18\n\x10\x63opy_annotations\x18\x03 \x01(\x08\x12\x13\n\x0b\x63opy_models\x18\x04 \x01(\x08\x12\x16\n\x0e\x63opy_workflows\x18\x05 \x01(\x08\"\xfa\x02\n\nLabelOrder\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x61uto_release\x18\x04 \x01(\x08\x12\x17\n\x0f\x61llow_empty_tag\x18\x05 \x01(\x08\x12\x38\n\x14\x64\x65sired_fulfill_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15\x65stimate_fulfill_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x04task\x18\x08 \x01(\x0b\x32\x12.clarifai.api.Task\x12.\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xbb\x06\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x04type\x18\x04 \x01(\x0e\x32\x1b.clarifai.api.Task.TaskType\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12(\n\x06worker\x18\x06 \x01(\x0b\x32\x18.clarifai.api.TaskWorker\x12\x17\n\x0b\x63oncept_ids\x18\x07 \x03(\tB\x02\x18\x01\x12\x33\n\x0cinput_source\x18\x08 \x01(\x0b\x32\x1d.clarifai.api.TaskInputSource\x12\x11\n\tsample_ms\x18\t \x01(\r\x12\x33\n\x0c\x61i_assistant\x18\n \x01(\x0b\x32\x1d.clarifai.api.TaskAIAssistant\x12(\n\x06review\x18\x0b \x01(\x0b\x32\x18.clarifai.api.TaskReview\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0c\n\x04name\x18\r \x01(\t\x12:\n\x10\x61i_assist_params\x18\x0e \x01(\x0b\x32 .clarifai.api.AiAssistParameters\x12,\n\nvisibility\x18\x0f \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06\x61pp_id\x18\x10 \x01(\t\x12\x0f\n\x07user_id\x18\x11 \x01(\t\x12\x16\n\x0elabel_order_id\x18\x12 \x01(\t\x12+\n\x08\x63oncepts\x18\x13 \x03(\x0b\x32\x19.clarifai.api.TaskConcept\x12#\n\x1b\x64\x65lete_previous_annotations\x18\x14 \x01(\x08\"l\n\x08TaskType\x12\x10\n\x0cTYPE_NOT_SET\x10\x00\x12\x1b\n\x17\x43ONCEPTS_CLASSIFICATION\x10\x01\x12\x1a\n\x16\x42OUNDING_BOX_DETECTION\x10\x02\x12\x15\n\x11POLYGON_DETECTION\x10\x03\"`\n\x12\x41iAssistParameters\x12\x15\n\rmin_threshold\x18\x01 \x01(\x02\x12\x15\n\rmax_threshold\x18\x02 \x01(\x02\x12\x1c\n\x14\x63oncept_relation_ids\x18\x03 \x03(\t\"\x8f\x03\n\nTaskWorker\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskWorker.TaskWorkerStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x04 \x03(\x0b\x32\x12.clarifai.api.User\x12#\n\x06models\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Model\x12)\n\tworkflows\x18\x06 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12T\n\x19partitioned_strategy_info\x18\x03 \x01(\x0b\x32/.clarifai.api.TaskWorkerPartitionedStrategyInfoH\x00\"R\n\x12TaskWorkerStrategy\x12\x1b\n\x17WORKER_STRATEGY_NOT_SET\x10\x00\x12\x0f\n\x0bPARTITIONED\x10\x02\x12\x08\n\x04\x46ULL\x10\x03\"\x04\x08\x01\x10\x01\x42\x0f\n\rstrategy_info\"\xa9\x02\n!TaskWorkerPartitionedStrategyInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.clarifai.api.TaskWorkerPartitionedStrategyInfo.TaskWorkerPartitionedStrategy\x12\x19\n\x11workers_per_input\x18\x02 \x01(\x05\x12(\n\x07weights\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"b\n\x1dTaskWorkerPartitionedStrategy\x12\'\n#PARTITIONED_WORKER_STRATEGY_NOT_SET\x10\x00\x12\n\n\x06\x45VENLY\x10\x01\x12\x0c\n\x08WEIGHTED\x10\x02\"\xc3\x01\n\x0fTaskInputSource\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.clarifai.api.TaskInputSource.TaskInputSourceType\x12\n\n\x02id\x18\x02 \x01(\t\"c\n\x13TaskInputSourceType\x12\x1d\n\x19INPUT_SOURCE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nALL_INPUTS\x10\x01\x12\x10\n\x0cSAVED_SEARCH\x10\x02\x12\x0b\n\x07\x44\x41TASET\x10\x03\"\x90\x03\n\nTaskReview\x12=\n\x08strategy\x18\x01 \x01(\x0e\x32+.clarifai.api.TaskReview.TaskReviewStrategy\x12\x14\n\x08user_ids\x18\x02 \x03(\tB\x02\x18\x01\x12!\n\x05users\x18\x05 \x03(\x0b\x32\x12.clarifai.api.User\x12J\n\x14manual_strategy_info\x18\x03 \x01(\x0b\x32*.clarifai.api.TaskReviewManualStrategyInfoH\x00\x12P\n\x17\x63onsensus_strategy_info\x18\x04 \x01(\x0b\x32-.clarifai.api.TaskReviewConsensusStrategyInfoH\x00\"[\n\x12TaskReviewStrategy\x12 \n\x1cTASK_REVIEW_STRATEGY_NOT_SET\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06MANUAL\x10\x02\x12\r\n\tCONSENSUS\x10\x03\x42\x0f\n\rstrategy_info\"9\n\x1cTaskReviewManualStrategyInfo\x12\x19\n\x11sample_percentage\x18\x01 \x01(\x02\"C\n\x1fTaskReviewConsensusStrategyInfo\x12\x1a\n\x12\x61pproval_threshold\x18\x02 \x01(\rJ\x04\x08\x01\x10\x02\"&\n\x0fTaskAIAssistant\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"\xbc\x01\n\x16TaskStatusCountPerUser\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x15\n\x07pending\x18\x02 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1d\n\x0f\x61waiting_review\x18\x03 \x01(\rB\x04\x80\xb5\x18\x01\x12\x15\n\x07success\x18\x04 \x01(\rB\x04\x80\xb5\x18\x01\x12\x1b\n\rreview_denied\x18\x05 \x01(\rB\x04\x80\xb5\x18\x01\x12\'\n\x19\x61waiting_consensus_review\x18\x06 \x01(\rB\x04\x80\xb5\x18\x01\"f\n\x0eThresholdRange\x12\x1a\n\x12is_lower_inclusive\x18\x01 \x01(\x08\x12\x1a\n\x12is_upper_inclusive\x18\x02 \x01(\x08\x12\r\n\x05lower\x18\x03 \x01(\x02\x12\r\n\x05upper\x18\x04 \x01(\x02\"\xad\x01\n\x1fTaskConceptAutoAnnotationConfig\x12\x1d\n\x15\x61nnotation_data_types\x18\x01 \x01(\r\x12\x35\n\x0fthreshold_range\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.ThresholdRange\x12\x34\n\x0bstatus_code\x18\x03 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\"\x84\x01\n\x0bTaskConcept\x12&\n\x07\x63oncept\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Concept\x12M\n\x16\x61uto_annotation_config\x18\x02 \x01(\x0b\x32-.clarifai.api.TaskConceptAutoAnnotationConfig\"\x81\x02\n\tCollector\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1d\n\x15pre_queue_workflow_id\x18\x04 \x01(\t\x12\x1e\n\x16post_queue_workflow_id\x18\x05 \x01(\t\x12\x37\n\x10\x63ollector_source\x18\x06 \x01(\x0b\x32\x1d.clarifai.api.CollectorSource\x12+\n\x06status\x18\x07 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"t\n\x0f\x43ollectorSource\x12\x61\n\'api_post_model_outputs_collector_source\x18\x02 \x01(\x0b\x32\x30.clarifai.api.APIPostModelOutputsCollectorSource\"\x99\x01\n\"APIPostModelOutputsCollectorSource\x12\x15\n\rmodel_user_id\x18\x01 \x01(\t\x12\x14\n\x0cmodel_app_id\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x18\n\x10model_version_id\x18\x04 \x01(\t\x12\x1a\n\x12post_inputs_key_id\x18\x05 \x01(\t\"R\n\tStatValue\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04tags\x18\x03 \x03(\t\"\xa6\x01\n\x18StatValueAggregateResult\x12?\n\x15stat_value_aggregates\x18\x01 \x03(\x0b\x32 .clarifai.api.StatValueAggregate\x12I\n\x1astat_value_aggregate_query\x18\x02 \x01(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"t\n\x12StatValueAggregate\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x61ggregate_value\x18\x02 \x01(\x02\x12\r\n\x05\x63ount\x18\x03 \x01(\x04\x12\x0c\n\x04tags\x18\x04 \x03(\t\"\x91\x02\n\x17StatValueAggregateQuery\x12\x0c\n\x04tags\x18\x01 \x03(\t\x12\x12\n\ntag_groups\x18\x02 \x03(\t\x12;\n\x13stat_value_agg_type\x18\x03 \x01(\x0e\x32\x1e.clarifai.api.StatValueAggType\x12\x39\n\x12stat_time_agg_type\x18\x04 \x01(\x0e\x32\x1d.clarifai.api.StatTimeAggType\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xef\x01\n\x19\x44\x61tasetInputsSearchAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x12\n\ndataset_id\x18\x05 \x01(\t\x12$\n\x06search\x18\x06 \x01(\x0b\x32\x14.clarifai.api.Search\"O\n\x17PCAProjectionComparator\x12\x1a\n\x12\x64istance_threshold\x18\x01 \x01(\x02\x12\x18\n\x10model_version_id\x18\x02 \x01(\t\"K\n\x1b\x44uplicateAnnotationsResults\x12\x16\n\x0e\x64uplicate_cfid\x18\x01 \x03(\t\x12\x14\n\x0cunique_count\x18\x02 \x01(\x05\"\x87\x01\n\nVisibility\x12\x33\n\x08gettable\x18\x01 \x01(\x0e\x32!.clarifai.api.Visibility.Gettable\"D\n\x08Gettable\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\x0b\n\x07PRIVATE\x10\n\x12\x07\n\x03ORG\x10\x1e\x12\n\n\x06PUBLIC\x10\x32\"X\n\x0eTrendingMetric\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\x12\x12\n\nview_count\x18\x04 \x01(\x04\"#\n\x07\x46ullTag\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x0bTimeSegment\x12\n\n\x02id\x18\x01 \x01(\t\x12 \n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Data\x12)\n\ttime_info\x18\x03 \x01(\x0b\x32\x16.clarifai.api.TimeInfo\"D\n\x08TimeInfo\x12\x12\n\nnum_frames\x18\x01 \x01(\r\x12\x12\n\nbegin_time\x18\x02 \x01(\r\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\r\"!\n\x0b\x44\x61tasetStar\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\x1f\n\nModuleStar\x12\x11\n\tmodule_id\x18\x01 \x01(\t\"\x9e\x03\n\x06Module\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\nvisibility\x18\x07 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\t \x01(\t\x12\x0e\n\x06\x61pp_id\x18\n \x01(\t\x12\x33\n\x0emodule_version\x18\x0b \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x12\n\nis_starred\x18\x0c \x01(\x08\x12\x12\n\nstar_count\x18\r \x01(\x05\x12\x35\n\x0f\x62ookmark_origin\x18\x0e \x01(\x0b\x32\x1c.clarifai.api.BookmarkOriginJ\x04\x08\x02\x10\x03\"\xbe\x04\n\rModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\r\n\x05notes\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0egit_commit_url\x18\n \x01(\t\x12\x39\n\nmodule_nav\x18\x0b \x01(\x0b\x32%.clarifai.api.ModuleVersion.ModuleNav\x12\x10\n\x08\x61pproved\x18\x0c \x01(\x08\x12,\n\nvisibility\x18\r \x01(\x0b\x32\x18.clarifai.api.Visibility\x12)\n\x08metadata\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\x1a\x45\n\x0cModuleSubNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x11\n\tquery_key\x18\x02 \x01(\t\x12\x13\n\x0bquery_value\x18\x03 \x01(\t\x1a]\n\tModuleNav\x12\r\n\x05title\x18\x01 \x01(\t\x12\x41\n\x0fmodule_sub_navs\x18\x02 \x03(\x0b\x32(.clarifai.api.ModuleVersion.ModuleSubNavJ\x04\x08\x05\x10\x06\"\xad\x02\n\x16InstalledModuleVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeploy_url\x18\x07 \x01(\t\x12,\n\nvisibility\x18\x08 \x01(\x0b\x32\x18.clarifai.api.Visibility\x12\x0e\n\x06key_id\x18\t \x01(\t\"\xb7\x03\n\rBulkOperation\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\tinput_ids\x18\x02 \x01(\x0b\x32\x16.clarifai.api.InputIDsH\x00\x12&\n\x06search\x18\n \x01(\x0b\x32\x14.clarifai.api.SearchH\x00\x12(\n\x07\x64\x61taset\x18\x0b \x01(\x0b\x32\x15.clarifai.api.DatasetH\x00\x12*\n\toperation\x18\x03 \x01(\x0b\x32\x17.clarifai.api.Operation\x12\x0e\n\x06\x61pp_id\x18\x04 \x01(\t\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08progress\x18\x06 \x01(\x0b\x32\x16.clarifai.api.Progress\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x0e\n\x0cinput_source\"\x1d\n\x08InputIDs\x12\x11\n\tinput_ids\x18\x01 \x03(\t\"8\n\x08Progress\x12\x11\n\tprocessed\x18\x01 \x01(\r\x12\x19\n\x11last_processed_id\x18\x02 \x01(\t\"\x8a\x04\n\tOperation\x12\x31\n\x0c\x61\x64\x64_concepts\x18\x01 \x01(\x0b\x32\x19.clarifai.api.AddConceptsH\x00\x12\x37\n\x0f\x64\x65lete_concepts\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DeleteConceptsH\x00\x12\x31\n\x0c\x61\x64\x64_metadata\x18\x03 \x01(\x0b\x32\x19.clarifai.api.AddMetadataH\x00\x12\x37\n\x0f\x64\x65lete_metadata\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.DeleteMetadataH\x00\x12\x33\n\roverwrite_geo\x18\x05 \x01(\x0b\x32\x1a.clarifai.api.OverwriteGeoH\x00\x12-\n\ndelete_geo\x18\x06 \x01(\x0b\x32\x17.clarifai.api.DeleteGeoH\x00\x12>\n\x13\x64\x65lete_from_dataset\x18\x07 \x01(\x0b\x32\x1f.clarifai.api.DeleteFromDatasetH\x00\x12\x34\n\x0e\x61\x64\x64_to_dataset\x18\x08 \x01(\x0b\x32\x1a.clarifai.api.AddToDatasetH\x00\x12>\n\x13split_into_datasets\x18\t \x01(\x0b\x32\x1f.clarifai.api.SplitIntoDatasetsH\x00\x42\x0b\n\toperation\"6\n\x0b\x41\x64\x64\x43oncepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\"K\n\x0e\x44\x65leteConcepts\x12\'\n\x08\x63oncepts\x18\x01 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x10\n\x08user_ids\x18\x02 \x03(\t\"8\n\x0b\x41\x64\x64Metadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\";\n\x0e\x44\x65leteMetadata\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\".\n\x0cOverwriteGeo\x12\x1e\n\x03geo\x18\x01 \x01(\x0b\x32\x11.clarifai.api.Geo\"\x0b\n\tDeleteGeo\"\"\n\x0c\x41\x64\x64ToDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\'\n\x11\x44\x65leteFromDataset\x12\x12\n\ndataset_id\x18\x01 \x01(\t\"\xcb\x01\n\x11SplitIntoDatasets\x12\x32\n\x0e\x64\x61taset_splits\x18\x01 \x03(\x0b\x32\x1a.clarifai.api.DatasetSplit\x12\x42\n\x06method\x18\x02 \x01(\x0e\x32\x32.clarifai.api.SplitIntoDatasets.DatasetSplitMethod\">\n\x12\x44\x61tasetSplitMethod\x12\x0b\n\x07NOT_SET\x10\x00\x12\x1b\n\x17RANDOM_PERCENTAGE_SPLIT\x10\x01\"[\n\x0c\x44\x61tasetSplit\x12&\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x15.clarifai.api.Dataset\x12\x14\n\npercentage\x18\x02 \x01(\rH\x00\x42\r\n\x0bmethod_info\"\xfb\x02\n\x0cInputsAddJob\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\x12\x34\n\x08progress\x18\x07 \x01(\x0b\x32\".clarifai.api.InputsAddJobProgress\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x0f\x65xtraction_jobs\x18\n \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\x12%\n\x07uploads\x18\x0b \x03(\x0b\x32\x14.clarifai.api.Upload\x12+\n\x06status\x18\x0c \x01(\x0b\x32\x1b.clarifai.api.status.StatusJ\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"u\n\x14InputsAddJobProgress\x12\x15\n\rpending_count\x18\x01 \x01(\x04\x12\x19\n\x11in_progress_count\x18\x02 \x01(\x04\x12\x15\n\rsuccess_count\x18\x03 \x01(\x04\x12\x14\n\x0c\x66\x61iled_count\x18\x04 \x01(\x04\"\x95\x02\n\x06Upload\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nexpires_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0c\x63ontent_name\x18\x08 \x01(\t\x12\x16\n\x0e\x63ontent_length\x18\x06 \x01(\x04\x12\x13\n\x0b\x63ontent_url\x18\x07 \x01(\t\"K\n\x11UploadContentPart\x12\x13\n\x0brange_start\x18\x01 \x01(\x04\x12\x13\n\x0bpart_number\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"l\n\x19\x43ustomCodeOperatorRequest\x12#\n\x06inputs\x18\x01 \x03(\x0b\x32\x13.clarifai.api.Input\x12*\n\x08metadata\x18\xea\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\"\xc8\x02\n\x13InputsExtractionJob\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12;\n\x08progress\x18\x04 \x01(\x0b\x32).clarifai.api.InputsExtractionJobProgress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12M\n\x1cinput_id_conflict_resolution\x18\x07 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"\x97\x02\n\x1bInputsExtractionJobProgress\x12\x1a\n\x12\x61udio_inputs_count\x18\x02 \x01(\x04\x12\x1a\n\x12image_inputs_count\x18\x03 \x01(\x04\x12\x1a\n\x12video_inputs_count\x18\x04 \x01(\x04\x12\x19\n\x11text_inputs_count\x18\x05 \x01(\x04\x12\x1e\n\x16pending_archives_count\x18\x06 \x01(\x04\x12\"\n\x1ain_progress_archives_count\x18\x07 \x01(\x04\x12 \n\x18\x63ompleted_archives_count\x18\x08 \x01(\x04\x12\x1d\n\x15\x66\x61iled_archives_count\x18\t \x01(\x04J\x04\x08\x01\x10\x02\"\xa6\x01\n\x10InputsDataSource\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12(\n\x03url\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.DataSourceURL\x12M\n\x1cinput_id_conflict_resolution\x18\x03 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"V\n\rDataSourceURL\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x38\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32#.clarifai.api.DataSourceCredentials\"\xa7\x01\n\x15\x44\x61taSourceCredentials\x12*\n\x08s3_creds\x18\x01 \x01(\x0b\x32\x16.clarifai.api.AWSCredsH\x00\x12\x13\n\tgcp_creds\x18\x02 \x01(\x0cH\x00\x12\x38\n\x10\x61zure_blob_creds\x18\x04 \x01(\x0b\x32\x1c.clarifai.api.AzureBlobCredsH\x00\x42\r\n\x0b\x63redentialsJ\x04\x08\x03\x10\x04\"K\n\x08\x41WSCreds\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12\x0e\n\x06secret\x18\x04 \x01(\t\x12\r\n\x05token\x18\x05 \x01(\tJ\x04\x08\x01\x10\x02\";\n\x0e\x41zureBlobCreds\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\"\xaf\x01\n\x0cInputsUpload\x12\x19\n\x11inputs_add_job_id\x18\x01 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x02 \x01(\t\x12$\n\x06upload\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Upload\x12M\n\x1cinput_id_conflict_resolution\x18\x04 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"\xce\x01\n\x0e\x42ookmarkOrigin\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\t\x12@\n\rresource_type\x18\x04 \x01(\x0e\x32).clarifai.api.BookmarkOrigin.BookmarkType\"M\n\x0c\x42ookmarkType\x12\x0b\n\x07unknown\x10\x00\x12\t\n\x05model\x10\x01\x12\x0c\n\x08workflow\x10\x02\x12\x0b\n\x07\x64\x61taset\x10\x03\x12\n\n\x06module\x10\x04\"\xd6\x01\n\x06Runner\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodified_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07user_id\x18\x06 \x01(\t\x12\x0e\n\x06labels\x18\x07 \x03(\t*\xf9\x01\n\x1e\x44\x61tasetVersionMetricsGroupType\x12.\n*DATASET_VERSION_METRICS_GROUP_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_TYPE\x10\x02\x12\x0e\n\nCONCEPT_ID\x10\n\x12\x12\n\x0e\x43ONCEPTS_COUNT\x10\x0b\x12\x18\n\x14\x42OUNDING_BOXES_COUNT\x10\x14\x12\x12\n\x0ePOLYGONS_COUNT\x10\x15\x12\x10\n\x0cPOINTS_COUNT\x10\x16\x12\x0f\n\x0bMASKS_COUNT\x10\x17\x12\x10\n\x0cPIXELS_COUNT\x10\x1e\x12\x10\n\x0c\x41SPECT_RATIO\x10\x1f*\x85\x01\n\x1a\x44\x61tasetVersionExportFormat\x12)\n%DATASET_VERSION_EXPORT_FORMAT_NOT_SET\x10\x00\x12\x1a\n\x16\x43LARIFAI_DATA_PROTOBUF\x10\x01\x12\x16\n\x12\x43LARIFAI_DATA_JSON\x10\x03\x12\x08\n\x04\x43OCO\x10\x02*H\n\x10\x45xpirationAction\x12\x1d\n\x19\x45XPIRATION_ACTION_NOT_SET\x10\x00\x12\t\n\x05\x44\x45LAY\x10\x01\x12\n\n\x06\x45XPIRY\x10\x02*M\n\x0cLicenseScope\x12\x19\n\x15LICENSE_SCOPE_NOT_SET\x10\x00\x12\x0b\n\x07PREDICT\x10\x01\x12\t\n\x05TRAIN\x10\x02\x12\n\n\x06SEARCH\x10\x03*P\n\x08\x44\x61taType\x12\r\n\tUNDEFINED\x10\x00\x12\n\n\x06STRING\x10\x01\x12\t\n\x05UINT8\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04\x46P32\x10\x05*\x8f\x01\n\x0fValueComparator\x12\x1d\n\x19\x43ONCEPT_THRESHOLD_NOT_SET\x10\x00\x12\x10\n\x0cGREATER_THAN\x10\x01\x12\x19\n\x15GREATER_THAN_OR_EQUAL\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x16\n\x12LESS_THAN_OR_EQUAL\x10\x04\x12\t\n\x05\x45QUAL\x10\x05*q\n\x0e\x45valuationType\x12\r\n\tUndefined\x10\x00\x12\x12\n\x0e\x43lassification\x10\x01\x12\r\n\tDetection\x10\x02\x12\x10\n\x0cSegmentation\x10\x03\x12\x0e\n\nClustering\x10\x04\x12\x0b\n\x07Tracker\x10\x05*f\n\x0c\x41PIEventType\x12\x1a\n\x16\x41PI_EVENT_TYPE_NOT_SET\x10\x00\x12\x13\n\x0fON_PREM_PREDICT\x10\x01\x12\x11\n\rON_PREM_TRAIN\x10\x02\x12\x12\n\x0eON_PREM_SEARCH\x10\x03*<\n\x11UsageIntervalType\x12\t\n\x05undef\x10\x00\x12\x07\n\x03\x64\x61y\x10\x01\x12\t\n\x05month\x10\x02\x12\x08\n\x04year\x10\x03*}\n\x12\x41nnotationDataType\x12 \n\x1c\x41NNOTATION_DATA_TYPE_NOT_SET\x10\x00\x12\x07\n\x03TAG\x10\x01\x12\x10\n\x0c\x42OUNDING_BOX\x10\x02\x12\x0b\n\x07POLYGON\x10\x04\x12\t\n\x05POINT\x10\x08\x12\x08\n\x04SPAN\x10\x10\x12\x08\n\x04MASK\x10 *\x1d\n\x08RoleType\x12\x08\n\x04TEAM\x10\x00\x12\x07\n\x03ORG\x10\x01*$\n\x10StatValueAggType\x12\x07\n\x03SUM\x10\x00\x12\x07\n\x03\x41VG\x10\x01*`\n\x0fStatTimeAggType\x12\x0f\n\x0bNO_TIME_AGG\x10\x00\x12\x08\n\x04YEAR\x10\x01\x12\t\n\x05MONTH\x10\x02\x12\x08\n\x04WEEK\x10\x03\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x05\x12\n\n\x06MINUTE\x10\x06*b\n\x13ValidationErrorType\x12!\n\x1dVALIDATION_ERROR_TYPE_NOT_SET\x10\x00\x12\x0e\n\nRESTRICTED\x10\x01\x12\x0c\n\x08\x44\x41TABASE\x10\x02\x12\n\n\x06\x46ORMAT\x10\x03*[\n\x19InputIDConflictResolution\x12(\n$INPUT_ID_CONFLICT_RESOLUTION_NOT_SET\x10\x00\x12\x08\n\x04SKIP\x10\x01\x12\n\n\x06SUFFIX\x10\x02\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.resources_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025com.clarifai.grpc.apiP\001Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\242\002\004CAIP'
@@ -121,14 +121,16 @@
   _OUTPUTCONFIG.fields_by_name['existing_model_id']._serialized_options = b'\030\001'
   _OUTPUTCONFIG.fields_by_name['hyper_parameters']._options = None
   _OUTPUTCONFIG.fields_by_name['hyper_parameters']._serialized_options = b'\030\001'
   _OUTPUTCONFIG.fields_by_name['max_concepts']._options = None
   _OUTPUTCONFIG.fields_by_name['max_concepts']._serialized_options = b'\200\265\030\001'
   _OUTPUTCONFIG.fields_by_name['min_value']._options = None
   _OUTPUTCONFIG.fields_by_name['min_value']._serialized_options = b'\200\265\030\001'
+  _OUTPUTCONFIG.fields_by_name['embed_model_version_id']._options = None
+  _OUTPUTCONFIG.fields_by_name['embed_model_version_id']._serialized_options = b'\030\001'
   _OUTPUTCONFIG.fields_by_name['model_metadata']._options = None
   _OUTPUTCONFIG.fields_by_name['model_metadata']._serialized_options = b'\030\001'
   _CONFUSIONMATRIXENTRY.fields_by_name['value']._options = None
   _CONFUSIONMATRIXENTRY.fields_by_name['value']._serialized_options = b'\200\265\030\001'
   _ROC.fields_by_name['fpr']._options = None
   _ROC.fields_by_name['fpr']._serialized_options = b'\200\265\030\001'
   _ROC.fields_by_name['tpr']._options = None
@@ -207,454 +209,462 @@
   _EMAILADDRESS.fields_by_name['primary']._serialized_options = b'\200\265\030\001'
   _EMAILADDRESS.fields_by_name['verified']._options = None
   _EMAILADDRESS.fields_by_name['verified']._serialized_options = b'\200\265\030\001'
   _WORKFLOW.fields_by_name['use_cases']._options = None
   _WORKFLOW.fields_by_name['use_cases']._serialized_options = b'\200\265\030\001'
   _WORKFLOW.fields_by_name['check_consents']._options = None
   _WORKFLOW.fields_by_name['check_consents']._serialized_options = b'\200\265\030\001'
+  _TASK.fields_by_name['concept_ids']._options = None
+  _TASK.fields_by_name['concept_ids']._serialized_options = b'\030\001'
   _TASKWORKER.fields_by_name['user_ids']._options = None
   _TASKWORKER.fields_by_name['user_ids']._serialized_options = b'\030\001'
   _TASKREVIEW.fields_by_name['user_ids']._options = None
   _TASKREVIEW.fields_by_name['user_ids']._serialized_options = b'\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['pending']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['pending']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_review']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_review']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['success']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['success']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['review_denied']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['review_denied']._serialized_options = b'\200\265\030\001'
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_consensus_review']._options = None
   _TASKSTATUSCOUNTPERUSER.fields_by_name['awaiting_consensus_review']._serialized_options = b'\200\265\030\001'
-  _DATASETVERSIONMETRICSGROUPTYPE._serialized_start=35866
-  _DATASETVERSIONMETRICSGROUPTYPE._serialized_end=36115
-  _DATASETVERSIONEXPORTFORMAT._serialized_start=36118
-  _DATASETVERSIONEXPORTFORMAT._serialized_end=36251
-  _EXPIRATIONACTION._serialized_start=36253
-  _EXPIRATIONACTION._serialized_end=36325
-  _LICENSESCOPE._serialized_start=36327
-  _LICENSESCOPE._serialized_end=36404
-  _DATATYPE._serialized_start=36406
-  _DATATYPE._serialized_end=36486
-  _VALUECOMPARATOR._serialized_start=36489
-  _VALUECOMPARATOR._serialized_end=36632
-  _EVALUATIONTYPE._serialized_start=36634
-  _EVALUATIONTYPE._serialized_end=36747
-  _APIEVENTTYPE._serialized_start=36749
-  _APIEVENTTYPE._serialized_end=36851
-  _USAGEINTERVALTYPE._serialized_start=36853
-  _USAGEINTERVALTYPE._serialized_end=36913
-  _ANNOTATIONDATATYPE._serialized_start=36915
-  _ANNOTATIONDATATYPE._serialized_end=37040
-  _ROLETYPE._serialized_start=37042
-  _ROLETYPE._serialized_end=37071
-  _STATVALUEAGGTYPE._serialized_start=37073
-  _STATVALUEAGGTYPE._serialized_end=37109
-  _STATTIMEAGGTYPE._serialized_start=37111
-  _STATTIMEAGGTYPE._serialized_end=37207
-  _VALIDATIONERRORTYPE._serialized_start=37209
-  _VALIDATIONERRORTYPE._serialized_end=37307
-  _INPUTIDCONFLICTRESOLUTION._serialized_start=37309
-  _INPUTIDCONFLICTRESOLUTION._serialized_end=37400
+  _DATASETVERSIONMETRICSGROUPTYPE._serialized_start=36703
+  _DATASETVERSIONMETRICSGROUPTYPE._serialized_end=36952
+  _DATASETVERSIONEXPORTFORMAT._serialized_start=36955
+  _DATASETVERSIONEXPORTFORMAT._serialized_end=37088
+  _EXPIRATIONACTION._serialized_start=37090
+  _EXPIRATIONACTION._serialized_end=37162
+  _LICENSESCOPE._serialized_start=37164
+  _LICENSESCOPE._serialized_end=37241
+  _DATATYPE._serialized_start=37243
+  _DATATYPE._serialized_end=37323
+  _VALUECOMPARATOR._serialized_start=37326
+  _VALUECOMPARATOR._serialized_end=37469
+  _EVALUATIONTYPE._serialized_start=37471
+  _EVALUATIONTYPE._serialized_end=37584
+  _APIEVENTTYPE._serialized_start=37586
+  _APIEVENTTYPE._serialized_end=37688
+  _USAGEINTERVALTYPE._serialized_start=37690
+  _USAGEINTERVALTYPE._serialized_end=37750
+  _ANNOTATIONDATATYPE._serialized_start=37752
+  _ANNOTATIONDATATYPE._serialized_end=37877
+  _ROLETYPE._serialized_start=37879
+  _ROLETYPE._serialized_end=37908
+  _STATVALUEAGGTYPE._serialized_start=37910
+  _STATVALUEAGGTYPE._serialized_end=37946
+  _STATTIMEAGGTYPE._serialized_start=37948
+  _STATTIMEAGGTYPE._serialized_end=38044
+  _VALIDATIONERRORTYPE._serialized_start=38046
+  _VALIDATIONERRORTYPE._serialized_end=38144
+  _INPUTIDCONFLICTRESOLUTION._serialized_start=38146
+  _INPUTIDCONFLICTRESOLUTION._serialized_end=38237
   _ANNOTATION._serialized_start=357
-  _ANNOTATION._serialized_end=842
-  _APP._serialized_start=845
-  _APP._serialized_end=1385
-  _APPQUERY._serialized_start=1387
-  _APPQUERY._serialized_end=1411
-  _COLLABORATOR._serialized_start=1414
-  _COLLABORATOR._serialized_end=1686
-  _COLLABORATION._serialized_start=1689
-  _COLLABORATION._serialized_end=1858
-  _AUDIO._serialized_start=1861
-  _AUDIO._serialized_end=2012
-  _AUDIOINFO._serialized_start=2014
-  _AUDIOINFO._serialized_end=2112
-  _TRACK._serialized_start=2114
-  _TRACK._serialized_end=2233
-  _CLUSTER._serialized_start=2235
-  _CLUSTER._serialized_end=2339
-  _COLOR._serialized_start=2341
-  _COLOR._serialized_end=2418
-  _W3C._serialized_start=2420
-  _W3C._serialized_end=2452
-  _USERAPPIDSET._serialized_start=2454
-  _USERAPPIDSET._serialized_end=2501
-  _PATCHACTION._serialized_start=2503
-  _PATCHACTION._serialized_end=2577
-  _CONCEPT._serialized_start=2580
-  _CONCEPT._serialized_end=2877
-  _KEYPOINTINFO._serialized_start=2879
-  _KEYPOINTINFO._serialized_end=2963
-  _KEYPOINTEDGE._serialized_start=2965
-  _KEYPOINTEDGE._serialized_end=3003
-  _CONCEPTCOUNT._serialized_start=3006
-  _CONCEPTCOUNT._serialized_end=3170
-  _CONCEPTTYPECOUNT._serialized_start=3172
-  _CONCEPTTYPECOUNT._serialized_end=3238
-  _DETAILCONCEPTCOUNT._serialized_start=3241
-  _DETAILCONCEPTCOUNT._serialized_end=3464
-  _CONCEPTQUERY._serialized_start=3466
-  _CONCEPTQUERY._serialized_end=3533
-  _CONCEPTRELATION._serialized_start=3536
-  _CONCEPTRELATION._serialized_end=3753
-  _KNOWLEDGEGRAPH._serialized_start=3755
-  _KNOWLEDGEGRAPH._serialized_end=3876
-  _CONCEPTMAPPINGJOB._serialized_start=3878
-  _CONCEPTMAPPINGJOB._serialized_end=3946
-  _CONCEPTLANGUAGE._serialized_start=3948
-  _CONCEPTLANGUAGE._serialized_end=4011
-  _DATA._serialized_start=4014
-  _DATA._serialized_end=4648
-  _REGION._serialized_start=4651
-  _REGION._serialized_end=4785
-  _REGIONINFO._serialized_start=4788
-  _REGIONINFO._serialized_end=5090
-  _BOUNDINGBOX._serialized_start=5092
-  _BOUNDINGBOX._serialized_end=5203
-  _FRAMEINFO._serialized_start=5205
-  _FRAMEINFO._serialized_end=5257
-  _FRAME._serialized_start=5259
-  _FRAME._serialized_end=5357
-  _MASK._serialized_start=5359
-  _MASK._serialized_end=5407
-  _POLYGON._serialized_start=5409
-  _POLYGON._serialized_end=5455
-  _POINT._serialized_start=5458
-  _POINT._serialized_end=5640
-  _POINT_VISIBILITY._serialized_start=5568
-  _POINT_VISIBILITY._serialized_end=5640
-  _SPAN._serialized_start=5642
-  _SPAN._serialized_end=5716
-  _TOKEN._serialized_start=5718
-  _TOKEN._serialized_end=5793
-  _EMBEDDING._serialized_start=5795
-  _EMBEDDING._serialized_end=5850
-  _GEOPOINT._serialized_start=5852
-  _GEOPOINT._serialized_end=5911
-  _GEOLIMIT._serialized_start=5913
-  _GEOLIMIT._serialized_end=5958
-  _GEOBOXEDPOINT._serialized_start=5960
-  _GEOBOXEDPOINT._serialized_end=6018
-  _GEO._serialized_start=6021
-  _GEO._serialized_end=6158
-  _IMAGE._serialized_start=6161
-  _IMAGE._serialized_end=6318
-  _IMAGEINFO._serialized_start=6320
-  _IMAGEINFO._serialized_end=6398
-  _HOSTEDURL._serialized_start=6400
-  _HOSTEDURL._serialized_end=6479
-  _INPUT._serialized_start=6482
-  _INPUT._serialized_end=6704
-  _INPUTBATCH._serialized_start=6706
-  _INPUTBATCH._serialized_end=6755
-  _INPUTCOUNT._serialized_start=6758
-  _INPUTCOUNT._serialized_end=6976
-  _DATASET._serialized_start=6979
-  _DATASET._serialized_end=7421
-  _ANNOTATIONFILTER._serialized_start=7424
-  _ANNOTATIONFILTER._serialized_end=7640
-  _DATASETINPUT._serialized_start=7642
-  _DATASETINPUT._serialized_end=7740
-  _DATASETVERSION._serialized_start=7743
-  _DATASETVERSION._serialized_end=8557
-  _DATASETVERSION_METRICSENTRY._serialized_start=8441
-  _DATASETVERSION_METRICSENTRY._serialized_end=8524
-  _ANNOTATIONFILTERCONFIG._serialized_start=8559
-  _ANNOTATIONFILTERCONFIG._serialized_end=8671
-  _MODELPREDICTCONFIG._serialized_start=8673
-  _MODELPREDICTCONFIG._serialized_end=8729
-  _DATASETVERSIONMETRICS._serialized_start=8732
-  _DATASETVERSIONMETRICS._serialized_end=9823
-  _DATASETVERSIONMETRICSGROUP._serialized_start=9826
-  _DATASETVERSIONMETRICSGROUP._serialized_end=10028
-  _DATASETVERSIONEXPORTINFO._serialized_start=10031
-  _DATASETVERSIONEXPORTINFO._serialized_end=10239
-  _DATASETVERSIONEXPORT._serialized_start=10242
-  _DATASETVERSIONEXPORT._serialized_end=10422
-  _DATASETVERSIONPROCESSINGINFO._serialized_start=10424
-  _DATASETVERSIONPROCESSINGINFO._serialized_end=10526
-  _FRAMEINTERPOLATIONINFO._serialized_start=10528
-  _FRAMEINTERPOLATIONINFO._serialized_end=10571
-  _WORKFLOWRESULTSSIMILARITY._serialized_start=10573
-  _WORKFLOWRESULTSSIMILARITY._serialized_end=10683
-  _KEY._serialized_start=10686
-  _KEY._serialized_end=10930
-  _MODEL._serialized_start=10933
-  _MODEL._serialized_end=11917
-  _MODELREFERENCE._serialized_start=11919
-  _MODELREFERENCE._serialized_end=12035
-  _MODELVERSIONINPUTEXAMPLE._serialized_start=12038
-  _MODELVERSIONINPUTEXAMPLE._serialized_end=12189
-  _OUTPUTINFO._serialized_start=12192
-  _OUTPUTINFO._serialized_end=12404
-  _INPUTINFO._serialized_start=12406
-  _INPUTINFO._serialized_end=12503
-  _TRAININFO._serialized_start=12505
-  _TRAININFO._serialized_end=12557
-  _EVALINFO._serialized_start=12559
-  _EVALINFO._serialized_end=12610
-  _IMPORTINFO._serialized_start=12612
-  _IMPORTINFO._serialized_end=12665
-  _OUTPUTCONFIG._serialized_start=12668
-  _OUTPUTCONFIG._serialized_end=13147
-  _MODELTYPE._serialized_start=13150
-  _MODELTYPE._serialized_end=13616
-  _MODELLAYERINFO._serialized_start=13619
-  _MODELLAYERINFO._serialized_end=13756
-  _TRITONCONDAENVINFO._serialized_start=13758
-  _TRITONCONDAENVINFO._serialized_end=13826
-  _LAYERSHAPE._serialized_start=13828
-  _LAYERSHAPE._serialized_end=13936
-  _MODELTYPEFIELD._serialized_start=13939
-  _MODELTYPEFIELD._serialized_end=14661
-  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_start=14304
-  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_end=14661
-  _MODELTYPERANGEINFO._serialized_start=14663
-  _MODELTYPERANGEINFO._serialized_end=14723
-  _MODELTYPEENUMOPTION._serialized_start=14726
-  _MODELTYPEENUMOPTION._serialized_end=14938
-  _MODELTYPEENUMOPTIONALIAS._serialized_start=14940
-  _MODELTYPEENUMOPTIONALIAS._serialized_end=15007
-  _MODELQUERY._serialized_start=15009
-  _MODELQUERY._serialized_end=15064
-  _MODELVERSION._serialized_start=15067
-  _MODELVERSION._serialized_end=15831
-  _PRETRAINEDMODELCONFIG._serialized_start=15834
-  _PRETRAINEDMODELCONFIG._serialized_end=15995
-  _TRAINSTATS._serialized_start=15997
-  _TRAINSTATS._serialized_end=16059
-  _LOSSCURVEENTRY._serialized_start=16061
-  _LOSSCURVEENTRY._serialized_end=16127
-  _LABELCOUNT._serialized_start=16129
-  _LABELCOUNT._serialized_end=16178
-  _LABELDISTRIBUTION._serialized_start=16180
-  _LABELDISTRIBUTION._serialized_end=16256
-  _COOCCURRENCEMATRIXENTRY._serialized_start=16258
-  _COOCCURRENCEMATRIXENTRY._serialized_end=16324
-  _COOCCURRENCEMATRIX._serialized_start=16326
-  _COOCCURRENCEMATRIX._serialized_end=16422
-  _CONFUSIONMATRIXENTRY._serialized_start=16424
-  _CONFUSIONMATRIXENTRY._serialized_end=16502
-  _CONFUSIONMATRIX._serialized_start=16504
-  _CONFUSIONMATRIX._serialized_end=16594
-  _ROC._serialized_start=16596
-  _ROC._serialized_end=16712
-  _PRECISIONRECALLCURVE._serialized_start=16714
-  _PRECISIONRECALLCURVE._serialized_end=16809
-  _BINARYMETRICS._serialized_start=16812
-  _BINARYMETRICS._serialized_end=17174
-  _TRACKERMETRICS._serialized_start=17177
-  _TRACKERMETRICS._serialized_end=17322
-  _EVALTESTSETENTRY._serialized_start=17325
-  _EVALTESTSETENTRY._serialized_end=17542
-  _LOPQEVALRESULT._serialized_start=17545
-  _LOPQEVALRESULT._serialized_end=17750
-  _METRICSSUMMARY._serialized_start=17753
-  _METRICSSUMMARY._serialized_end=18149
-  _EVALMETRICS._serialized_start=18152
-  _EVALMETRICS._serialized_end=18876
-  _FIELDSVALUE._serialized_start=18879
-  _FIELDSVALUE._serialized_end=19062
-  _OUTPUT._serialized_start=19065
-  _OUTPUT._serialized_end=19284
-  _SCOPEDEPS._serialized_start=19286
-  _SCOPEDEPS._serialized_end=19338
-  _ENDPOINTDEPS._serialized_start=19340
-  _ENDPOINTDEPS._serialized_end=19398
-  _HIT._serialized_start=19401
-  _HIT._serialized_end=19542
-  _HITCOUNT._serialized_start=19544
-  _HITCOUNT._serialized_end=19579
-  _AND._serialized_start=19582
-  _AND._serialized_end=19723
-  _QUERY._serialized_start=19726
-  _QUERY._serialized_end=19862
-  _SEARCH._serialized_start=19865
-  _SEARCH._serialized_end=20335
-  _SEARCH_METRIC._serialized_start=20262
-  _SEARCH_METRIC._serialized_end=20335
-  _FILTER._serialized_start=20338
-  _FILTER._serialized_end=20502
-  _TIMERANGE._serialized_start=20504
-  _TIMERANGE._serialized_end=20609
-  _RANK._serialized_start=20611
-  _RANK._serialized_end=20679
-  _ANNOTATIONSEARCHMETRICS._serialized_start=20682
-  _ANNOTATIONSEARCHMETRICS._serialized_end=20951
-  _TEXT._serialized_start=20954
-  _TEXT._serialized_end=21099
-  _TEXTINFO._serialized_start=21101
-  _TEXTINFO._serialized_end=21149
-  _USER._serialized_start=21152
-  _USER._serialized_end=21916
-  _USERDETAIL._serialized_start=21919
-  _USERDETAIL._serialized_end=22384
-  _EMAILADDRESS._serialized_start=22386
-  _EMAILADDRESS._serialized_end=22468
-  _PASSWORD._serialized_start=22470
-  _PASSWORD._serialized_end=22499
-  _PASSWORDVIOLATIONS._serialized_start=22502
-  _PASSWORDVIOLATIONS._serialized_end=22892
-  _VIDEO._serialized_start=22895
-  _VIDEO._serialized_end=23069
-  _VIDEOINFO._serialized_start=23072
-  _VIDEOINFO._serialized_end=23214
-  _WORKFLOW._serialized_start=23217
-  _WORKFLOW._serialized_end=23680
-  _WORKFLOWVERSION._serialized_start=23683
-  _WORKFLOWVERSION._serialized_end=24033
-  _WORKFLOWNODE._serialized_start=24036
-  _WORKFLOWNODE._serialized_end=24225
-  _NODEINPUT._serialized_start=24227
-  _NODEINPUT._serialized_end=24255
-  _WORKFLOWRESULT._serialized_start=24258
-  _WORKFLOWRESULT._serialized_end=24515
-  _WORKFLOWSTATE._serialized_start=24517
-  _WORKFLOWSTATE._serialized_end=24544
-  _APPDUPLICATION._serialized_start=24547
-  _APPDUPLICATION._serialized_end=24891
-  _APPCOPYPROGRESS._serialized_start=24893
-  _APPCOPYPROGRESS._serialized_end=24940
-  _APPDUPLICATIONFILTERS._serialized_start=24943
-  _APPDUPLICATIONFILTERS._serialized_end=25081
-  _LABELORDER._serialized_start=25084
-  _LABELORDER._serialized_end=25462
-  _TASK._serialized_start=25465
-  _TASK._serialized_end=26288
-  _TASK_TASKTYPE._serialized_start=26180
-  _TASK_TASKTYPE._serialized_end=26288
-  _AIASSISTPARAMETERS._serialized_start=26290
-  _AIASSISTPARAMETERS._serialized_end=26386
-  _TASKWORKER._serialized_start=26389
-  _TASKWORKER._serialized_end=26788
-  _TASKWORKER_TASKWORKERSTRATEGY._serialized_start=26689
-  _TASKWORKER_TASKWORKERSTRATEGY._serialized_end=26771
-  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_start=26791
-  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_end=27088
-  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_start=26990
-  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_end=27088
-  _TASKINPUTSOURCE._serialized_start=27091
-  _TASKINPUTSOURCE._serialized_end=27286
-  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_start=27187
-  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_end=27286
-  _TASKREVIEW._serialized_start=27289
-  _TASKREVIEW._serialized_end=27689
-  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_start=27581
-  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_end=27672
-  _TASKREVIEWMANUALSTRATEGYINFO._serialized_start=27691
-  _TASKREVIEWMANUALSTRATEGYINFO._serialized_end=27748
-  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_start=27750
-  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_end=27817
-  _TASKAIASSISTANT._serialized_start=27819
-  _TASKAIASSISTANT._serialized_end=27857
-  _TASKSTATUSCOUNTPERUSER._serialized_start=27860
-  _TASKSTATUSCOUNTPERUSER._serialized_end=28048
-  _THRESHOLDRANGE._serialized_start=28050
-  _THRESHOLDRANGE._serialized_end=28152
-  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_start=28155
-  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_end=28328
-  _TASKCONCEPT._serialized_start=28331
-  _TASKCONCEPT._serialized_end=28463
-  _COLLECTOR._serialized_start=28466
-  _COLLECTOR._serialized_end=28723
-  _COLLECTORSOURCE._serialized_start=28725
-  _COLLECTORSOURCE._serialized_end=28841
-  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_start=28844
-  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_end=28997
-  _STATVALUE._serialized_start=28999
-  _STATVALUE._serialized_end=29081
-  _STATVALUEAGGREGATERESULT._serialized_start=29084
-  _STATVALUEAGGREGATERESULT._serialized_end=29250
-  _STATVALUEAGGREGATE._serialized_start=29252
-  _STATVALUEAGGREGATE._serialized_end=29368
-  _STATVALUEAGGREGATEQUERY._serialized_start=29371
-  _STATVALUEAGGREGATEQUERY._serialized_end=29644
-  _DATASETINPUTSSEARCHADDJOB._serialized_start=29647
-  _DATASETINPUTSSEARCHADDJOB._serialized_end=29886
-  _PCAPROJECTIONCOMPARATOR._serialized_start=29888
-  _PCAPROJECTIONCOMPARATOR._serialized_end=29967
-  _DUPLICATEANNOTATIONSRESULTS._serialized_start=29969
-  _DUPLICATEANNOTATIONSRESULTS._serialized_end=30044
-  _VISIBILITY._serialized_start=30047
-  _VISIBILITY._serialized_end=30182
-  _VISIBILITY_GETTABLE._serialized_start=30114
-  _VISIBILITY_GETTABLE._serialized_end=30182
-  _TRENDINGMETRIC._serialized_start=30184
-  _TRENDINGMETRIC._serialized_end=30272
-  _FULLTAG._serialized_start=30274
-  _FULLTAG._serialized_end=30309
-  _TIMESEGMENT._serialized_start=30311
-  _TIMESEGMENT._serialized_end=30413
-  _TIMEINFO._serialized_start=30415
-  _TIMEINFO._serialized_end=30483
-  _DATASETSTAR._serialized_start=30485
-  _DATASETSTAR._serialized_end=30518
-  _MODULESTAR._serialized_start=30520
-  _MODULESTAR._serialized_end=30551
-  _MODULE._serialized_start=30554
-  _MODULE._serialized_end=30913
-  _MODULEVERSION._serialized_start=30916
-  _MODULEVERSION._serialized_end=31490
-  _MODULEVERSION_MODULESUBNAV._serialized_start=31320
-  _MODULEVERSION_MODULESUBNAV._serialized_end=31389
-  _MODULEVERSION_MODULENAV._serialized_start=31391
-  _MODULEVERSION_MODULENAV._serialized_end=31484
-  _INSTALLEDMODULEVERSION._serialized_start=31493
-  _INSTALLEDMODULEVERSION._serialized_end=31794
-  _BULKOPERATION._serialized_start=31797
-  _BULKOPERATION._serialized_end=32236
-  _INPUTIDS._serialized_start=32238
-  _INPUTIDS._serialized_end=32267
-  _PROGRESS._serialized_start=32269
-  _PROGRESS._serialized_end=32325
-  _OPERATION._serialized_start=32328
-  _OPERATION._serialized_end=32850
-  _ADDCONCEPTS._serialized_start=32852
-  _ADDCONCEPTS._serialized_end=32906
-  _DELETECONCEPTS._serialized_start=32908
-  _DELETECONCEPTS._serialized_end=32983
-  _ADDMETADATA._serialized_start=32985
-  _ADDMETADATA._serialized_end=33041
-  _DELETEMETADATA._serialized_start=33043
-  _DELETEMETADATA._serialized_end=33102
-  _OVERWRITEGEO._serialized_start=33104
-  _OVERWRITEGEO._serialized_end=33150
-  _DELETEGEO._serialized_start=33152
-  _DELETEGEO._serialized_end=33163
-  _ADDTODATASET._serialized_start=33165
-  _ADDTODATASET._serialized_end=33199
-  _DELETEFROMDATASET._serialized_start=33201
-  _DELETEFROMDATASET._serialized_end=33240
-  _SPLITINTODATASETS._serialized_start=33243
-  _SPLITINTODATASETS._serialized_end=33446
-  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_start=33384
-  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_end=33446
-  _DATASETSPLIT._serialized_start=33448
-  _DATASETSPLIT._serialized_end=33539
-  _INPUTSADDJOB._serialized_start=33542
-  _INPUTSADDJOB._serialized_end=33921
-  _INPUTSADDJOBPROGRESS._serialized_start=33923
-  _INPUTSADDJOBPROGRESS._serialized_end=34040
-  _UPLOAD._serialized_start=34043
-  _UPLOAD._serialized_end=34320
-  _UPLOADCONTENTPART._serialized_start=34322
-  _UPLOADCONTENTPART._serialized_end=34397
-  _CUSTOMCODEOPERATORREQUEST._serialized_start=34399
-  _CUSTOMCODEOPERATORREQUEST._serialized_end=34507
-  _INPUTSEXTRACTIONJOB._serialized_start=34510
-  _INPUTSEXTRACTIONJOB._serialized_end=34838
-  _INPUTSEXTRACTIONJOBPROGRESS._serialized_start=34841
-  _INPUTSEXTRACTIONJOBPROGRESS._serialized_end=35120
-  _INPUTSDATASOURCE._serialized_start=35123
-  _INPUTSDATASOURCE._serialized_end=35289
-  _DATASOURCEURL._serialized_start=35291
-  _DATASOURCEURL._serialized_end=35377
-  _DATASOURCECREDENTIALS._serialized_start=35380
-  _DATASOURCECREDENTIALS._serialized_end=35547
-  _AWSCREDS._serialized_start=35549
-  _AWSCREDS._serialized_end=35624
-  _AZUREBLOBCREDS._serialized_start=35626
-  _AZUREBLOBCREDS._serialized_end=35685
-  _INPUTSUPLOAD._serialized_start=35688
-  _INPUTSUPLOAD._serialized_end=35863
+  _ANNOTATION._serialized_end=871
+  _APP._serialized_start=874
+  _APP._serialized_end=1414
+  _APPQUERY._serialized_start=1416
+  _APPQUERY._serialized_end=1440
+  _COLLABORATOR._serialized_start=1443
+  _COLLABORATOR._serialized_end=1715
+  _COLLABORATION._serialized_start=1718
+  _COLLABORATION._serialized_end=1887
+  _AUDIO._serialized_start=1890
+  _AUDIO._serialized_end=2041
+  _AUDIOINFO._serialized_start=2043
+  _AUDIOINFO._serialized_end=2141
+  _TRACK._serialized_start=2143
+  _TRACK._serialized_end=2262
+  _CLUSTER._serialized_start=2264
+  _CLUSTER._serialized_end=2368
+  _COLOR._serialized_start=2370
+  _COLOR._serialized_end=2447
+  _W3C._serialized_start=2449
+  _W3C._serialized_end=2481
+  _USERAPPIDSET._serialized_start=2483
+  _USERAPPIDSET._serialized_end=2530
+  _PATCHACTION._serialized_start=2532
+  _PATCHACTION._serialized_end=2606
+  _CONCEPT._serialized_start=2609
+  _CONCEPT._serialized_end=2906
+  _KEYPOINTINFO._serialized_start=2908
+  _KEYPOINTINFO._serialized_end=2992
+  _KEYPOINTEDGE._serialized_start=2994
+  _KEYPOINTEDGE._serialized_end=3032
+  _CONCEPTCOUNT._serialized_start=3035
+  _CONCEPTCOUNT._serialized_end=3199
+  _CONCEPTTYPECOUNT._serialized_start=3201
+  _CONCEPTTYPECOUNT._serialized_end=3267
+  _DETAILCONCEPTCOUNT._serialized_start=3270
+  _DETAILCONCEPTCOUNT._serialized_end=3493
+  _CONCEPTQUERY._serialized_start=3495
+  _CONCEPTQUERY._serialized_end=3562
+  _CONCEPTRELATION._serialized_start=3565
+  _CONCEPTRELATION._serialized_end=3782
+  _KNOWLEDGEGRAPH._serialized_start=3784
+  _KNOWLEDGEGRAPH._serialized_end=3905
+  _CONCEPTMAPPINGJOB._serialized_start=3907
+  _CONCEPTMAPPINGJOB._serialized_end=3975
+  _CONCEPTLANGUAGE._serialized_start=3977
+  _CONCEPTLANGUAGE._serialized_end=4040
+  _DATA._serialized_start=4043
+  _DATA._serialized_end=4677
+  _REGION._serialized_start=4680
+  _REGION._serialized_end=4814
+  _REGIONINFO._serialized_start=4817
+  _REGIONINFO._serialized_end=5119
+  _BOUNDINGBOX._serialized_start=5121
+  _BOUNDINGBOX._serialized_end=5232
+  _FRAMEINFO._serialized_start=5234
+  _FRAMEINFO._serialized_end=5286
+  _FRAME._serialized_start=5288
+  _FRAME._serialized_end=5386
+  _MASK._serialized_start=5388
+  _MASK._serialized_end=5436
+  _POLYGON._serialized_start=5438
+  _POLYGON._serialized_end=5484
+  _POINT._serialized_start=5487
+  _POINT._serialized_end=5669
+  _POINT_VISIBILITY._serialized_start=5597
+  _POINT_VISIBILITY._serialized_end=5669
+  _SPAN._serialized_start=5671
+  _SPAN._serialized_end=5745
+  _TOKEN._serialized_start=5747
+  _TOKEN._serialized_end=5822
+  _EMBEDDING._serialized_start=5824
+  _EMBEDDING._serialized_end=5879
+  _GEOPOINT._serialized_start=5881
+  _GEOPOINT._serialized_end=5940
+  _GEOLIMIT._serialized_start=5942
+  _GEOLIMIT._serialized_end=5987
+  _GEOBOXEDPOINT._serialized_start=5989
+  _GEOBOXEDPOINT._serialized_end=6047
+  _GEO._serialized_start=6050
+  _GEO._serialized_end=6187
+  _IMAGE._serialized_start=6190
+  _IMAGE._serialized_end=6347
+  _IMAGEINFO._serialized_start=6349
+  _IMAGEINFO._serialized_end=6427
+  _HOSTEDURL._serialized_start=6429
+  _HOSTEDURL._serialized_end=6508
+  _INPUT._serialized_start=6511
+  _INPUT._serialized_end=6733
+  _INPUTBATCH._serialized_start=6735
+  _INPUTBATCH._serialized_end=6784
+  _INPUTCOUNT._serialized_start=6787
+  _INPUTCOUNT._serialized_end=7005
+  _DATASET._serialized_start=7008
+  _DATASET._serialized_end=7582
+  _ANNOTATIONFILTER._serialized_start=7585
+  _ANNOTATIONFILTER._serialized_end=7801
+  _DATASETINPUT._serialized_start=7803
+  _DATASETINPUT._serialized_end=7901
+  _DATASETVERSION._serialized_start=7904
+  _DATASETVERSION._serialized_end=8718
+  _DATASETVERSION_METRICSENTRY._serialized_start=8602
+  _DATASETVERSION_METRICSENTRY._serialized_end=8685
+  _ANNOTATIONFILTERCONFIG._serialized_start=8720
+  _ANNOTATIONFILTERCONFIG._serialized_end=8832
+  _MODELPREDICTCONFIG._serialized_start=8834
+  _MODELPREDICTCONFIG._serialized_end=8890
+  _DATASETVERSIONMETRICS._serialized_start=8893
+  _DATASETVERSIONMETRICS._serialized_end=9984
+  _DATASETVERSIONMETRICSGROUP._serialized_start=9987
+  _DATASETVERSIONMETRICSGROUP._serialized_end=10189
+  _DATASETVERSIONEXPORTINFO._serialized_start=10192
+  _DATASETVERSIONEXPORTINFO._serialized_end=10400
+  _DATASETVERSIONEXPORT._serialized_start=10403
+  _DATASETVERSIONEXPORT._serialized_end=10583
+  _DATASETVERSIONPROCESSINGINFO._serialized_start=10585
+  _DATASETVERSIONPROCESSINGINFO._serialized_end=10687
+  _FRAMEINTERPOLATIONINFO._serialized_start=10689
+  _FRAMEINTERPOLATIONINFO._serialized_end=10732
+  _WORKFLOWRESULTSSIMILARITY._serialized_start=10734
+  _WORKFLOWRESULTSSIMILARITY._serialized_end=10844
+  _KEY._serialized_start=10847
+  _KEY._serialized_end=11091
+  _MODEL._serialized_start=11094
+  _MODEL._serialized_end=12133
+  _MODELREFERENCE._serialized_start=12135
+  _MODELREFERENCE._serialized_end=12251
+  _MODELVERSIONINPUTEXAMPLE._serialized_start=12254
+  _MODELVERSIONINPUTEXAMPLE._serialized_end=12405
+  _OUTPUTINFO._serialized_start=12408
+  _OUTPUTINFO._serialized_end=12620
+  _INPUTINFO._serialized_start=12623
+  _INPUTINFO._serialized_end=12767
+  _TRAININFO._serialized_start=12769
+  _TRAININFO._serialized_end=12821
+  _EVALINFO._serialized_start=12823
+  _EVALINFO._serialized_end=12874
+  _IMPORTINFO._serialized_start=12876
+  _IMPORTINFO._serialized_end=12929
+  _OUTPUTCONFIG._serialized_start=12932
+  _OUTPUTCONFIG._serialized_end=13415
+  _MODELTYPE._serialized_start=13418
+  _MODELTYPE._serialized_end=13884
+  _MODELLAYERINFO._serialized_start=13887
+  _MODELLAYERINFO._serialized_end=14024
+  _TRITONCONDAENVINFO._serialized_start=14026
+  _TRITONCONDAENVINFO._serialized_end=14094
+  _LAYERSHAPE._serialized_start=14096
+  _LAYERSHAPE._serialized_end=14204
+  _MODELTYPEFIELD._serialized_start=14207
+  _MODELTYPEFIELD._serialized_end=14958
+  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_start=14572
+  _MODELTYPEFIELD_MODELTYPEFIELDTYPE._serialized_end=14958
+  _MODELTYPERANGEINFO._serialized_start=14960
+  _MODELTYPERANGEINFO._serialized_end=15020
+  _MODELTYPEENUMOPTION._serialized_start=15023
+  _MODELTYPEENUMOPTION._serialized_end=15235
+  _MODELTYPEENUMOPTIONALIAS._serialized_start=15237
+  _MODELTYPEENUMOPTIONALIAS._serialized_end=15304
+  _MODELQUERY._serialized_start=15306
+  _MODELQUERY._serialized_end=15361
+  _MODELVERSION._serialized_start=15364
+  _MODELVERSION._serialized_end=16128
+  _PRETRAINEDMODELCONFIG._serialized_start=16131
+  _PRETRAINEDMODELCONFIG._serialized_end=16292
+  _TRAINSTATS._serialized_start=16294
+  _TRAINSTATS._serialized_end=16356
+  _LOSSCURVEENTRY._serialized_start=16358
+  _LOSSCURVEENTRY._serialized_end=16424
+  _LABELCOUNT._serialized_start=16426
+  _LABELCOUNT._serialized_end=16475
+  _LABELDISTRIBUTION._serialized_start=16477
+  _LABELDISTRIBUTION._serialized_end=16553
+  _COOCCURRENCEMATRIXENTRY._serialized_start=16555
+  _COOCCURRENCEMATRIXENTRY._serialized_end=16621
+  _COOCCURRENCEMATRIX._serialized_start=16623
+  _COOCCURRENCEMATRIX._serialized_end=16719
+  _CONFUSIONMATRIXENTRY._serialized_start=16721
+  _CONFUSIONMATRIXENTRY._serialized_end=16799
+  _CONFUSIONMATRIX._serialized_start=16801
+  _CONFUSIONMATRIX._serialized_end=16891
+  _ROC._serialized_start=16893
+  _ROC._serialized_end=17009
+  _PRECISIONRECALLCURVE._serialized_start=17011
+  _PRECISIONRECALLCURVE._serialized_end=17106
+  _BINARYMETRICS._serialized_start=17109
+  _BINARYMETRICS._serialized_end=17471
+  _TRACKERMETRICS._serialized_start=17474
+  _TRACKERMETRICS._serialized_end=17619
+  _EVALTESTSETENTRY._serialized_start=17622
+  _EVALTESTSETENTRY._serialized_end=17839
+  _LOPQEVALRESULT._serialized_start=17842
+  _LOPQEVALRESULT._serialized_end=18047
+  _METRICSSUMMARY._serialized_start=18050
+  _METRICSSUMMARY._serialized_end=18446
+  _EVALMETRICS._serialized_start=18449
+  _EVALMETRICS._serialized_end=19173
+  _FIELDSVALUE._serialized_start=19176
+  _FIELDSVALUE._serialized_end=19359
+  _OUTPUT._serialized_start=19362
+  _OUTPUT._serialized_end=19581
+  _SCOPEDEPS._serialized_start=19583
+  _SCOPEDEPS._serialized_end=19635
+  _ENDPOINTDEPS._serialized_start=19637
+  _ENDPOINTDEPS._serialized_end=19695
+  _HIT._serialized_start=19698
+  _HIT._serialized_end=19839
+  _HITCOUNT._serialized_start=19841
+  _HITCOUNT._serialized_end=19876
+  _AND._serialized_start=19879
+  _AND._serialized_end=20020
+  _QUERY._serialized_start=20023
+  _QUERY._serialized_end=20159
+  _SEARCH._serialized_start=20162
+  _SEARCH._serialized_end=20632
+  _SEARCH_METRIC._serialized_start=20559
+  _SEARCH_METRIC._serialized_end=20632
+  _FILTER._serialized_start=20635
+  _FILTER._serialized_end=20799
+  _TIMERANGE._serialized_start=20801
+  _TIMERANGE._serialized_end=20906
+  _RANK._serialized_start=20908
+  _RANK._serialized_end=20976
+  _ANNOTATIONSEARCHMETRICS._serialized_start=20979
+  _ANNOTATIONSEARCHMETRICS._serialized_end=21248
+  _TEXT._serialized_start=21251
+  _TEXT._serialized_end=21396
+  _TEXTINFO._serialized_start=21398
+  _TEXTINFO._serialized_end=21446
+  _USER._serialized_start=21449
+  _USER._serialized_end=22213
+  _USERDETAIL._serialized_start=22216
+  _USERDETAIL._serialized_end=22681
+  _EMAILADDRESS._serialized_start=22683
+  _EMAILADDRESS._serialized_end=22765
+  _PASSWORD._serialized_start=22767
+  _PASSWORD._serialized_end=22796
+  _PASSWORDVIOLATIONS._serialized_start=22799
+  _PASSWORDVIOLATIONS._serialized_end=23189
+  _VIDEO._serialized_start=23192
+  _VIDEO._serialized_end=23366
+  _VIDEOINFO._serialized_start=23369
+  _VIDEOINFO._serialized_end=23511
+  _WORKFLOW._serialized_start=23514
+  _WORKFLOW._serialized_end=24032
+  _WORKFLOWVERSION._serialized_start=24035
+  _WORKFLOWVERSION._serialized_end=24385
+  _WORKFLOWNODE._serialized_start=24388
+  _WORKFLOWNODE._serialized_end=24577
+  _NODEINPUT._serialized_start=24579
+  _NODEINPUT._serialized_end=24607
+  _WORKFLOWRESULT._serialized_start=24610
+  _WORKFLOWRESULT._serialized_end=24867
+  _WORKFLOWSTATE._serialized_start=24869
+  _WORKFLOWSTATE._serialized_end=24896
+  _APPDUPLICATION._serialized_start=24899
+  _APPDUPLICATION._serialized_end=25243
+  _APPCOPYPROGRESS._serialized_start=25245
+  _APPCOPYPROGRESS._serialized_end=25292
+  _APPDUPLICATIONFILTERS._serialized_start=25295
+  _APPDUPLICATIONFILTERS._serialized_end=25433
+  _LABELORDER._serialized_start=25436
+  _LABELORDER._serialized_end=25814
+  _TASK._serialized_start=25817
+  _TASK._serialized_end=26644
+  _TASK_TASKTYPE._serialized_start=26536
+  _TASK_TASKTYPE._serialized_end=26644
+  _AIASSISTPARAMETERS._serialized_start=26646
+  _AIASSISTPARAMETERS._serialized_end=26742
+  _TASKWORKER._serialized_start=26745
+  _TASKWORKER._serialized_end=27144
+  _TASKWORKER_TASKWORKERSTRATEGY._serialized_start=27045
+  _TASKWORKER_TASKWORKERSTRATEGY._serialized_end=27127
+  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_start=27147
+  _TASKWORKERPARTITIONEDSTRATEGYINFO._serialized_end=27444
+  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_start=27346
+  _TASKWORKERPARTITIONEDSTRATEGYINFO_TASKWORKERPARTITIONEDSTRATEGY._serialized_end=27444
+  _TASKINPUTSOURCE._serialized_start=27447
+  _TASKINPUTSOURCE._serialized_end=27642
+  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_start=27543
+  _TASKINPUTSOURCE_TASKINPUTSOURCETYPE._serialized_end=27642
+  _TASKREVIEW._serialized_start=27645
+  _TASKREVIEW._serialized_end=28045
+  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_start=27937
+  _TASKREVIEW_TASKREVIEWSTRATEGY._serialized_end=28028
+  _TASKREVIEWMANUALSTRATEGYINFO._serialized_start=28047
+  _TASKREVIEWMANUALSTRATEGYINFO._serialized_end=28104
+  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_start=28106
+  _TASKREVIEWCONSENSUSSTRATEGYINFO._serialized_end=28173
+  _TASKAIASSISTANT._serialized_start=28175
+  _TASKAIASSISTANT._serialized_end=28213
+  _TASKSTATUSCOUNTPERUSER._serialized_start=28216
+  _TASKSTATUSCOUNTPERUSER._serialized_end=28404
+  _THRESHOLDRANGE._serialized_start=28406
+  _THRESHOLDRANGE._serialized_end=28508
+  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_start=28511
+  _TASKCONCEPTAUTOANNOTATIONCONFIG._serialized_end=28684
+  _TASKCONCEPT._serialized_start=28687
+  _TASKCONCEPT._serialized_end=28819
+  _COLLECTOR._serialized_start=28822
+  _COLLECTOR._serialized_end=29079
+  _COLLECTORSOURCE._serialized_start=29081
+  _COLLECTORSOURCE._serialized_end=29197
+  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_start=29200
+  _APIPOSTMODELOUTPUTSCOLLECTORSOURCE._serialized_end=29353
+  _STATVALUE._serialized_start=29355
+  _STATVALUE._serialized_end=29437
+  _STATVALUEAGGREGATERESULT._serialized_start=29440
+  _STATVALUEAGGREGATERESULT._serialized_end=29606
+  _STATVALUEAGGREGATE._serialized_start=29608
+  _STATVALUEAGGREGATE._serialized_end=29724
+  _STATVALUEAGGREGATEQUERY._serialized_start=29727
+  _STATVALUEAGGREGATEQUERY._serialized_end=30000
+  _DATASETINPUTSSEARCHADDJOB._serialized_start=30003
+  _DATASETINPUTSSEARCHADDJOB._serialized_end=30242
+  _PCAPROJECTIONCOMPARATOR._serialized_start=30244
+  _PCAPROJECTIONCOMPARATOR._serialized_end=30323
+  _DUPLICATEANNOTATIONSRESULTS._serialized_start=30325
+  _DUPLICATEANNOTATIONSRESULTS._serialized_end=30400
+  _VISIBILITY._serialized_start=30403
+  _VISIBILITY._serialized_end=30538
+  _VISIBILITY_GETTABLE._serialized_start=30470
+  _VISIBILITY_GETTABLE._serialized_end=30538
+  _TRENDINGMETRIC._serialized_start=30540
+  _TRENDINGMETRIC._serialized_end=30628
+  _FULLTAG._serialized_start=30630
+  _FULLTAG._serialized_end=30665
+  _TIMESEGMENT._serialized_start=30667
+  _TIMESEGMENT._serialized_end=30769
+  _TIMEINFO._serialized_start=30771
+  _TIMEINFO._serialized_end=30839
+  _DATASETSTAR._serialized_start=30841
+  _DATASETSTAR._serialized_end=30874
+  _MODULESTAR._serialized_start=30876
+  _MODULESTAR._serialized_end=30907
+  _MODULE._serialized_start=30910
+  _MODULE._serialized_end=31324
+  _MODULEVERSION._serialized_start=31327
+  _MODULEVERSION._serialized_end=31901
+  _MODULEVERSION_MODULESUBNAV._serialized_start=31731
+  _MODULEVERSION_MODULESUBNAV._serialized_end=31800
+  _MODULEVERSION_MODULENAV._serialized_start=31802
+  _MODULEVERSION_MODULENAV._serialized_end=31895
+  _INSTALLEDMODULEVERSION._serialized_start=31904
+  _INSTALLEDMODULEVERSION._serialized_end=32205
+  _BULKOPERATION._serialized_start=32208
+  _BULKOPERATION._serialized_end=32647
+  _INPUTIDS._serialized_start=32649
+  _INPUTIDS._serialized_end=32678
+  _PROGRESS._serialized_start=32680
+  _PROGRESS._serialized_end=32736
+  _OPERATION._serialized_start=32739
+  _OPERATION._serialized_end=33261
+  _ADDCONCEPTS._serialized_start=33263
+  _ADDCONCEPTS._serialized_end=33317
+  _DELETECONCEPTS._serialized_start=33319
+  _DELETECONCEPTS._serialized_end=33394
+  _ADDMETADATA._serialized_start=33396
+  _ADDMETADATA._serialized_end=33452
+  _DELETEMETADATA._serialized_start=33454
+  _DELETEMETADATA._serialized_end=33513
+  _OVERWRITEGEO._serialized_start=33515
+  _OVERWRITEGEO._serialized_end=33561
+  _DELETEGEO._serialized_start=33563
+  _DELETEGEO._serialized_end=33574
+  _ADDTODATASET._serialized_start=33576
+  _ADDTODATASET._serialized_end=33610
+  _DELETEFROMDATASET._serialized_start=33612
+  _DELETEFROMDATASET._serialized_end=33651
+  _SPLITINTODATASETS._serialized_start=33654
+  _SPLITINTODATASETS._serialized_end=33857
+  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_start=33795
+  _SPLITINTODATASETS_DATASETSPLITMETHOD._serialized_end=33857
+  _DATASETSPLIT._serialized_start=33859
+  _DATASETSPLIT._serialized_end=33950
+  _INPUTSADDJOB._serialized_start=33953
+  _INPUTSADDJOB._serialized_end=34332
+  _INPUTSADDJOBPROGRESS._serialized_start=34334
+  _INPUTSADDJOBPROGRESS._serialized_end=34451
+  _UPLOAD._serialized_start=34454
+  _UPLOAD._serialized_end=34731
+  _UPLOADCONTENTPART._serialized_start=34733
+  _UPLOADCONTENTPART._serialized_end=34808
+  _CUSTOMCODEOPERATORREQUEST._serialized_start=34810
+  _CUSTOMCODEOPERATORREQUEST._serialized_end=34918
+  _INPUTSEXTRACTIONJOB._serialized_start=34921
+  _INPUTSEXTRACTIONJOB._serialized_end=35249
+  _INPUTSEXTRACTIONJOBPROGRESS._serialized_start=35252
+  _INPUTSEXTRACTIONJOBPROGRESS._serialized_end=35531
+  _INPUTSDATASOURCE._serialized_start=35534
+  _INPUTSDATASOURCE._serialized_end=35700
+  _DATASOURCEURL._serialized_start=35702
+  _DATASOURCEURL._serialized_end=35788
+  _DATASOURCECREDENTIALS._serialized_start=35791
+  _DATASOURCECREDENTIALS._serialized_end=35958
+  _AWSCREDS._serialized_start=35960
+  _AWSCREDS._serialized_end=36035
+  _AZUREBLOBCREDS._serialized_start=36037
+  _AZUREBLOBCREDS._serialized_end=36096
+  _INPUTSUPLOAD._serialized_start=36099
+  _INPUTSUPLOAD._serialized_end=36274
+  _BOOKMARKORIGIN._serialized_start=36277
+  _BOOKMARKORIGIN._serialized_end=36483
+  _BOOKMARKORIGIN_BOOKMARKTYPE._serialized_start=36406
+  _BOOKMARKORIGIN_BOOKMARKTYPE._serialized_end=36483
+  _RUNNER._serialized_start=36486
+  _RUNNER._serialized_end=36700
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/resources_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/resources_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -463,14 +463,15 @@
     STATUS_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     MODIFIED_AT_FIELD_NUMBER: builtins.int
     TRUSTED_FIELD_NUMBER: builtins.int
     INPUT_LEVEL_FIELD_NUMBER: builtins.int
     CONSENSUS_INFO_FIELD_NUMBER: builtins.int
     TASK_ID_FIELD_NUMBER: builtins.int
+    WORKFLOW_VERSION_ID_FIELD_NUMBER: builtins.int
     id: builtins.str
     """The ID for the annotation"""
     input_id: builtins.str
     """ID of the input this annotation is tied to"""
     @property
     def data(self) -> global___Data:
         """The data passed along in this annotation."""
@@ -507,14 +508,16 @@
     def consensus_info(self) -> google.protobuf.struct_pb2.Struct:
         """Consensus review related information, e.g.
         * annotation group
         * id of annotation parent, in case the annotation was split from another annotation
         """
     task_id: builtins.str
     """The id of the task annotation belongs to"""
+    workflow_version_id: builtins.str
+    """ID of the workflow version this annotation is created by"""
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         input_id: builtins.str = ...,
         data: global___Data | None = ...,
         annotation_info: google.protobuf.struct_pb2.Struct | None = ...,
@@ -524,17 +527,18 @@
         status: proto.clarifai.api.status.status_pb2.Status | None = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         trusted: builtins.bool = ...,
         input_level: builtins.bool = ...,
         consensus_info: google.protobuf.struct_pb2.Struct | None = ...,
         task_id: builtins.str = ...,
+        workflow_version_id: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["annotation_info", b"annotation_info", "consensus_info", b"consensus_info", "created_at", b"created_at", "data", b"data", "modified_at", b"modified_at", "status", b"status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotation_info", b"annotation_info", "consensus_info", b"consensus_info", "created_at", b"created_at", "data", b"data", "embed_model_version_id", b"embed_model_version_id", "id", b"id", "input_id", b"input_id", "input_level", b"input_level", "model_version_id", b"model_version_id", "modified_at", b"modified_at", "status", b"status", "task_id", b"task_id", "trusted", b"trusted", "user_id", b"user_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["annotation_info", b"annotation_info", "consensus_info", b"consensus_info", "created_at", b"created_at", "data", b"data", "embed_model_version_id", b"embed_model_version_id", "id", b"id", "input_id", b"input_id", "input_level", b"input_level", "model_version_id", b"model_version_id", "modified_at", b"modified_at", "status", b"status", "task_id", b"task_id", "trusted", b"trusted", "user_id", b"user_id", "workflow_version_id", b"workflow_version_id"]) -> None: ...
 
 global___Annotation = Annotation
 
 @typing_extensions.final
 class App(google.protobuf.message.Message):
     """Application with tasks and datasets"""
 
@@ -2223,18 +2227,20 @@
     MODIFIED_AT_FIELD_NUMBER: builtins.int
     APP_ID_FIELD_NUMBER: builtins.int
     USER_ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     VISIBILITY_FIELD_NUMBER: builtins.int
     DEFAULT_ANNOTATION_FILTER_FIELD_NUMBER: builtins.int
+    DEFAULT_PROCESSING_INFO_FIELD_NUMBER: builtins.int
     NOTES_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     IS_STARRED_FIELD_NUMBER: builtins.int
     STAR_COUNT_FIELD_NUMBER: builtins.int
+    BOOKMARK_ORIGIN_FIELD_NUMBER: builtins.int
     id: builtins.str
     """The ID for the dataset"""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """When the dataset was created.
         The format is https://www.ietf.org/rfc/rfc3339.txt.
         Example: "2006-01-02T15:04:05.999999Z".
@@ -2261,46 +2267,56 @@
         """The visibility field represents whether this message is privately/publicly visible.
         To be visible to the public the App that contains it AND the User that contains the App must
         also be publicly visible.
         """
     @property
     def default_annotation_filter(self) -> global___AnnotationFilter:
         """Default annotation filter used for this dataset."""
+    @property
+    def default_processing_info(self) -> global___DatasetVersionProcessingInfo:
+        """Default processing info used for this dataset."""
     notes: builtins.str
     """Notes for the dataset
     This field should be used for in-depth notes and supports up to 64Kbs.
     """
     @property
     def version(self) -> global___DatasetVersion:
         """Dataset version associated with this dataset. This is used in listing Datasets
         and including the latest version.
         """
     is_starred: builtins.bool
     """Whether the dataset is starred by the requesting user."""
     star_count: builtins.int
     """Number of users that starred this dataset."""
+    @property
+    def bookmark_origin(self) -> global___BookmarkOrigin:
+        """bookmark info. When set, this dataset is a bookmarked dataset of this app.
+        Info in this field will allow you to find/access original dataset.
+        """
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         app_id: builtins.str = ...,
         user_id: builtins.str = ...,
         description: builtins.str = ...,
         metadata: google.protobuf.struct_pb2.Struct | None = ...,
         visibility: global___Visibility | None = ...,
         default_annotation_filter: global___AnnotationFilter | None = ...,
+        default_processing_info: global___DatasetVersionProcessingInfo | None = ...,
         notes: builtins.str = ...,
         version: global___DatasetVersion | None = ...,
         is_starred: builtins.bool = ...,
         star_count: builtins.int = ...,
+        bookmark_origin: global___BookmarkOrigin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "default_annotation_filter", b"default_annotation_filter", "metadata", b"metadata", "modified_at", b"modified_at", "version", b"version", "visibility", b"visibility"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "created_at", b"created_at", "default_annotation_filter", b"default_annotation_filter", "description", b"description", "id", b"id", "is_starred", b"is_starred", "metadata", b"metadata", "modified_at", b"modified_at", "notes", b"notes", "star_count", b"star_count", "user_id", b"user_id", "version", b"version", "visibility", b"visibility"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["bookmark_origin", b"bookmark_origin", "created_at", b"created_at", "default_annotation_filter", b"default_annotation_filter", "default_processing_info", b"default_processing_info", "metadata", b"metadata", "modified_at", b"modified_at", "version", b"version", "visibility", b"visibility"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "bookmark_origin", b"bookmark_origin", "created_at", b"created_at", "default_annotation_filter", b"default_annotation_filter", "default_processing_info", b"default_processing_info", "description", b"description", "id", b"id", "is_starred", b"is_starred", "metadata", b"metadata", "modified_at", b"modified_at", "notes", b"notes", "star_count", b"star_count", "user_id", b"user_id", "version", b"version", "visibility", b"visibility"]) -> None: ...
 
 global___Dataset = Dataset
 
 @typing_extensions.final
 class AnnotationFilter(google.protobuf.message.Message):
     """AnnotationFilter is used to create a new dataset version.
     For now, the filter is simply a wrapper over a Search.
@@ -2448,15 +2464,18 @@
     @property
     def status(self) -> proto.clarifai.api.status.status_pb2.Status:
         """Status for this dataset version."""
     description: builtins.str
     """Description of the dataset version"""
     @property
     def processing_info(self) -> global___DatasetVersionProcessingInfo:
-        """Dataset version processing"""
+        """Dataset version processing. If this is not set when the dataset version is
+        created, then the dataset default_processing_info is copied instead. Later
+        updates to default_processing_info will not apply to existing versions.
+        """
     @property
     def metrics(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___DatasetVersionMetrics]:
         """Dataset version metrics"""
     @property
     def export_info(self) -> global___DatasetVersionExportInfo:
         """Dataset version exports"""
     @property
@@ -2761,14 +2780,18 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FRAME_INTERPOLATION_INFO_FIELD_NUMBER: builtins.int
     @property
     def frame_interpolation_info(self) -> global___FrameInterpolationInfo:
         """If frame_interpolation_info is set, then these settings are used to
         interpolate new frame annotation from other video annotations.
+
+        If frame_interpolation_info is set in the dataset default_processing_info,
+        then it can be disabled for a single dataset version by setting
+        processing_info but not setting processing_info.frame_interpolation_info.
         """
     def __init__(
         self,
         *,
         frame_interpolation_info: global___FrameInterpolationInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["frame_interpolation_info", b"frame_interpolation_info"]) -> builtins.bool: ...
@@ -2784,15 +2807,17 @@
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SAMPLE_MS_FIELD_NUMBER: builtins.int
     sample_ms: builtins.int
     """sample_ms is the sampling rate at which frame annotations are interpolated.
-    If zero, then the input frame prediction sampling rate is used.
+    If sample_ms is zero, then the dataset default_processing_info value is used.
+    If the dataset default is zero or not set, then the input frame prediction
+    sampling rate is used.
     """
     def __init__(
         self,
         *,
         sample_ms: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["sample_ms", b"sample_ms"]) -> None: ...
@@ -2928,14 +2953,15 @@
     LANGUAGES_FIELD_NUMBER: builtins.int
     LANGUAGES_FULL_FIELD_NUMBER: builtins.int
     CHECK_CONSENTS_FIELD_NUMBER: builtins.int
     IS_STARRED_FIELD_NUMBER: builtins.int
     STAR_COUNT_FIELD_NUMBER: builtins.int
     IMPORT_INFO_FIELD_NUMBER: builtins.int
     WORKFLOW_RECOMMENDED_FIELD_NUMBER: builtins.int
+    BOOKMARK_ORIGIN_FIELD_NUMBER: builtins.int
     id: builtins.str
     """The model's ID. Must be unique within a particular app and URL-friendly."""
     name: builtins.str
     """DEPRECATED: Please use the model id to name the model."""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """When the model was created. We follow the XXXX timestamp
@@ -3027,14 +3053,19 @@
     def import_info(self) -> global___ImportInfo:
         """Configuration used to import model from third-party toolkits
         DEPRECATED: Will be moved to model version
         """
     @property
     def workflow_recommended(self) -> google.protobuf.wrappers_pb2.BoolValue:
         """Whether it's recommended that this model is used within a workflow"""
+    @property
+    def bookmark_origin(self) -> global___BookmarkOrigin:
+        """bookmark info. When set, this model is a bookmarked model of this app.
+        Info in this field will allow you to find/access original model.
+        """
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         name: builtins.str = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
@@ -3058,17 +3089,18 @@
         languages: collections.abc.Iterable[builtins.str] | None = ...,
         languages_full: collections.abc.Iterable[global___FullTag] | None = ...,
         check_consents: collections.abc.Iterable[builtins.str] | None = ...,
         is_starred: builtins.bool = ...,
         star_count: builtins.int = ...,
         import_info: global___ImportInfo | None = ...,
         workflow_recommended: google.protobuf.wrappers_pb2.BoolValue | None = ...,
+        bookmark_origin: global___BookmarkOrigin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "default_eval_info", b"default_eval_info", "import_info", b"import_info", "input_info", b"input_info", "metadata", b"metadata", "model_version", b"model_version", "modified_at", b"modified_at", "output_info", b"output_info", "presets", b"presets", "train_info", b"train_info", "visibility", b"visibility", "workflow_recommended", b"workflow_recommended"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "check_consents", b"check_consents", "created_at", b"created_at", "default_eval_info", b"default_eval_info", "description", b"description", "display_name", b"display_name", "id", b"id", "import_info", b"import_info", "input_info", b"input_info", "is_starred", b"is_starred", "languages", b"languages", "languages_full", b"languages_full", "metadata", b"metadata", "model_type_id", b"model_type_id", "model_version", b"model_version", "modified_at", b"modified_at", "name", b"name", "notes", b"notes", "output_info", b"output_info", "presets", b"presets", "star_count", b"star_count", "task", b"task", "toolkits", b"toolkits", "train_info", b"train_info", "use_cases", b"use_cases", "user_id", b"user_id", "visibility", b"visibility", "workflow_recommended", b"workflow_recommended"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["bookmark_origin", b"bookmark_origin", "created_at", b"created_at", "default_eval_info", b"default_eval_info", "import_info", b"import_info", "input_info", b"input_info", "metadata", b"metadata", "model_version", b"model_version", "modified_at", b"modified_at", "output_info", b"output_info", "presets", b"presets", "train_info", b"train_info", "visibility", b"visibility", "workflow_recommended", b"workflow_recommended"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "bookmark_origin", b"bookmark_origin", "check_consents", b"check_consents", "created_at", b"created_at", "default_eval_info", b"default_eval_info", "description", b"description", "display_name", b"display_name", "id", b"id", "import_info", b"import_info", "input_info", b"input_info", "is_starred", b"is_starred", "languages", b"languages", "languages_full", b"languages_full", "metadata", b"metadata", "model_type_id", b"model_type_id", "model_version", b"model_version", "modified_at", b"modified_at", "name", b"name", "notes", b"notes", "output_info", b"output_info", "presets", b"presets", "star_count", b"star_count", "task", b"task", "toolkits", b"toolkits", "train_info", b"train_info", "use_cases", b"use_cases", "user_id", b"user_id", "visibility", b"visibility", "workflow_recommended", b"workflow_recommended"]) -> None: ...
 
 global___Model = Model
 
 @typing_extensions.final
 class ModelReference(google.protobuf.message.Message):
     """A link to a html/markdown/text file that stores reference material tied to a model."""
 
@@ -3204,33 +3236,38 @@
 class InputInfo(google.protobuf.message.Message):
     """InputInfo"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FIELDS_MAP_FIELD_NUMBER: builtins.int
     PARAMS_FIELD_NUMBER: builtins.int
+    BASE_EMBED_MODEL_FIELD_NUMBER: builtins.int
     @property
     def fields_map(self) -> google.protobuf.struct_pb2.Struct:
         """Map from the api.Data field names to the underlying model graph's inputs. When using a
         PretrainedModelConfig the values in this map need to match the Triton config.pbtxt input names.
         """
     @property
     def params(self) -> google.protobuf.struct_pb2.Struct:
         """To control the inputs to the given model we allow a list of parameters
         defined for each ModelType as a Struct (JSON object) here. During training or inference, the
         settings contained within are sent to the training processor to alter the training process.
         """
+    @property
+    def base_embed_model(self) -> global___Model:
+        """For base model to get embeddings from for transfer learned models."""
     def __init__(
         self,
         *,
         fields_map: google.protobuf.struct_pb2.Struct | None = ...,
         params: google.protobuf.struct_pb2.Struct | None = ...,
+        base_embed_model: global___Model | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["fields_map", b"fields_map", "params", b"params"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fields_map", b"fields_map", "params", b"params"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["base_embed_model", b"base_embed_model", "fields_map", b"fields_map", "params", b"params"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["base_embed_model", b"base_embed_model", "fields_map", b"fields_map", "params", b"params"]) -> None: ...
 
 global___InputInfo = InputInfo
 
 @typing_extensions.final
 class TrainInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -3342,14 +3379,15 @@
     """For model predictions on video: Sample delay for video predicting (1 frame per N milliseconds)"""
     @property
     def hyper_params(self) -> google.protobuf.struct_pb2.Struct:
         """For custom model training: Hyperparameters for custom training"""
     embed_model_version_id: builtins.str
     """For custom model training: this is the base model version to use for image embeddings.
     This has to be one of the embed models in the app workflow.
+    Use input_info.base_embed_model instead.
     """
     fail_on_missing_positive_examples: builtins.bool
     """For custom model training: Use this flag to fail on missing positive examples
     By default we fill in the missing with random examples
     """
     @property
     def model_metadata(self) -> google.protobuf.struct_pb2.Struct:
@@ -3594,14 +3632,16 @@
         """
         PYTHON_CODE: ModelTypeField._ModelTypeFieldType.ValueType  # 15
         """For blocks of code that need to be specified by the user for setup or execution during workflow runs."""
         DATASET_ID: ModelTypeField._ModelTypeFieldType.ValueType  # 16
         """For selecting a dataset id in model parameters. String in API request."""
         DATASET_VERSION_ID: ModelTypeField._ModelTypeFieldType.ValueType  # 17
         """For selecting a dataset version id. String."""
+        ARRAY_OF_MODEL_CONCEPTS: ModelTypeField._ModelTypeFieldType.ValueType  # 18
+        """For auto-completing to concepts in the model."""
 
     class ModelTypeFieldType(_ModelTypeFieldType, metaclass=_ModelTypeFieldTypeEnumTypeWrapper):
         """These are various types of fields that we have UIs for."""
 
     INVALID_MODEL_TYPE_FIELD_TYPE: ModelTypeField.ModelTypeFieldType.ValueType  # 0
     BOOLEAN: ModelTypeField.ModelTypeFieldType.ValueType  # 1
     STRING: ModelTypeField.ModelTypeFieldType.ValueType  # 2
@@ -3634,14 +3674,16 @@
     """
     PYTHON_CODE: ModelTypeField.ModelTypeFieldType.ValueType  # 15
     """For blocks of code that need to be specified by the user for setup or execution during workflow runs."""
     DATASET_ID: ModelTypeField.ModelTypeFieldType.ValueType  # 16
     """For selecting a dataset id in model parameters. String in API request."""
     DATASET_VERSION_ID: ModelTypeField.ModelTypeFieldType.ValueType  # 17
     """For selecting a dataset version id. String."""
+    ARRAY_OF_MODEL_CONCEPTS: ModelTypeField.ModelTypeFieldType.ValueType  # 18
+    """For auto-completing to concepts in the model."""
 
     PATH_FIELD_NUMBER: builtins.int
     FIELD_TYPE_FIELD_NUMBER: builtins.int
     DEFAULT_VALUE_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     PLACEHOLDER_FIELD_NUMBER: builtins.int
     MODEL_TYPE_ENUM_OPTIONS_FIELD_NUMBER: builtins.int
@@ -5048,17 +5090,19 @@
          - data.regions[].region_info.polygon - filter by polygon annotations
          - data.regions[].region_info.span - filter by span annotations
          - data.text - filter by text annotations
          - data.time_segments[].time_info - filter by time-segment annotations
          - id
          - input_id
          - input_level
+         - model_version_id
          - status.code
          - task_id
          - user_id
+         - workflow_version_id
         """
     @property
     def input(self) -> global___Input:
         """FILTER by input information.
         ########## Supported fields ##########
          - data.audio - filter audio inputs
          - data.image - filter image inputs
@@ -5644,14 +5688,15 @@
     VERSION_FIELD_NUMBER: builtins.int
     IS_STARRED_FIELD_NUMBER: builtins.int
     STAR_COUNT_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     NOTES_FIELD_NUMBER: builtins.int
     USE_CASES_FIELD_NUMBER: builtins.int
     CHECK_CONSENTS_FIELD_NUMBER: builtins.int
+    BOOKMARK_ORIGIN_FIELD_NUMBER: builtins.int
     id: builtins.str
     """The workflows's unique id."""
     app_id: builtins.str
     """The app the workflow belongs to"""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """When the workflow was created. We follow the XXXX timestamp
@@ -5700,14 +5745,19 @@
     """
     @property
     def use_cases(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Tags from use_cases category"""
     @property
     def check_consents(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Tags for check consents"""
+    @property
+    def bookmark_origin(self) -> global___BookmarkOrigin:
+        """bookmark info. When set, this workflow is a bookmarked workflow of this app.
+        Info in this field will allow you to find/access original workflow.
+        """
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         app_id: builtins.str = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         nodes: collections.abc.Iterable[global___WorkflowNode] | None = ...,
@@ -5718,17 +5768,18 @@
         version: global___WorkflowVersion | None = ...,
         is_starred: builtins.bool = ...,
         star_count: builtins.int = ...,
         description: builtins.str = ...,
         notes: builtins.str = ...,
         use_cases: collections.abc.Iterable[builtins.str] | None = ...,
         check_consents: collections.abc.Iterable[builtins.str] | None = ...,
+        bookmark_origin: global___BookmarkOrigin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "metadata", b"metadata", "modified_at", b"modified_at", "version", b"version", "visibility", b"visibility"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "check_consents", b"check_consents", "created_at", b"created_at", "description", b"description", "id", b"id", "is_starred", b"is_starred", "metadata", b"metadata", "modified_at", b"modified_at", "nodes", b"nodes", "notes", b"notes", "star_count", b"star_count", "use_cases", b"use_cases", "user_id", b"user_id", "version", b"version", "visibility", b"visibility"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["bookmark_origin", b"bookmark_origin", "created_at", b"created_at", "metadata", b"metadata", "modified_at", b"modified_at", "version", b"version", "visibility", b"visibility"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "bookmark_origin", b"bookmark_origin", "check_consents", b"check_consents", "created_at", b"created_at", "description", b"description", "id", b"id", "is_starred", b"is_starred", "metadata", b"metadata", "modified_at", b"modified_at", "nodes", b"nodes", "notes", b"notes", "star_count", b"star_count", "use_cases", b"use_cases", "user_id", b"user_id", "version", b"version", "visibility", b"visibility"]) -> None: ...
 
 global___Workflow = Workflow
 
 @typing_extensions.final
 class WorkflowVersion(google.protobuf.message.Message):
     """WorkflowVersion"""
 
@@ -6195,15 +6246,17 @@
     description: builtins.str
     """Description of the task."""
     @property
     def worker(self) -> global___TaskWorker:
         """Worker details."""
     @property
     def concept_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """List of concept ids used in the work of this task if label type is classification."""
+        """List of concept ids used in the work of this task.
+        DEPRECATED: Use task.concepts instead.
+        """
     @property
     def input_source(self) -> global___TaskInputSource:
         """List of inputs used in this task will be taken from this source."""
     sample_ms: builtins.int
     """For model predictions on video: Sample delay for video predicting (1 frame per N milliseconds)"""
     @property
     def ai_assistant(self) -> global___TaskAIAssistant:
@@ -7317,14 +7370,15 @@
     VISIBILITY_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     USER_ID_FIELD_NUMBER: builtins.int
     APP_ID_FIELD_NUMBER: builtins.int
     MODULE_VERSION_FIELD_NUMBER: builtins.int
     IS_STARRED_FIELD_NUMBER: builtins.int
     STAR_COUNT_FIELD_NUMBER: builtins.int
+    BOOKMARK_ORIGIN_FIELD_NUMBER: builtins.int
     id: builtins.str
     """A unique ID for this app module."""
     description: builtins.str
     """A short description for this app module to be used in grids of modules."""
     @property
     def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """When the app module was created."""
@@ -7357,31 +7411,37 @@
     """Is starred by the requesting user (only showed on get/list requests)
     Please use PostModuleStars/DeleteModuleStars endpoints to star/unstar a module
     """
     star_count: builtins.int
     """How many users have starred the module (only showed on get/list requests)
     Computed value, not editable
     """
+    @property
+    def bookmark_origin(self) -> global___BookmarkOrigin:
+        """bookmark info. When set, this module is a bookmarked module of this app.
+        Info in this field will allow you to find/access original module.
+        """
     def __init__(
         self,
         *,
         id: builtins.str = ...,
         description: builtins.str = ...,
         created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         visibility: global___Visibility | None = ...,
         metadata: google.protobuf.struct_pb2.Struct | None = ...,
         user_id: builtins.str = ...,
         app_id: builtins.str = ...,
         module_version: global___ModuleVersion | None = ...,
         is_starred: builtins.bool = ...,
         star_count: builtins.int = ...,
+        bookmark_origin: global___BookmarkOrigin | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "metadata", b"metadata", "modified_at", b"modified_at", "module_version", b"module_version", "visibility", b"visibility"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "created_at", b"created_at", "description", b"description", "id", b"id", "is_starred", b"is_starred", "metadata", b"metadata", "modified_at", b"modified_at", "module_version", b"module_version", "star_count", b"star_count", "user_id", b"user_id", "visibility", b"visibility"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["bookmark_origin", b"bookmark_origin", "created_at", b"created_at", "metadata", b"metadata", "modified_at", b"modified_at", "module_version", b"module_version", "visibility", b"visibility"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "bookmark_origin", b"bookmark_origin", "created_at", b"created_at", "description", b"description", "id", b"id", "is_starred", b"is_starred", "metadata", b"metadata", "modified_at", b"modified_at", "module_version", b"module_version", "star_count", b"star_count", "user_id", b"user_id", "visibility", b"visibility"]) -> None: ...
 
 global___Module = Module
 
 @typing_extensions.final
 class ModuleVersion(google.protobuf.message.Message):
     """A specific version of an app module that is available for assigning to apps."""
 
@@ -8380,7 +8440,104 @@
         upload: global___Upload | None = ...,
         input_id_conflict_resolution: global___InputIDConflictResolution.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["upload", b"upload"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_pat", b"app_pat", "input_id_conflict_resolution", b"input_id_conflict_resolution", "inputs_add_job_id", b"inputs_add_job_id", "upload", b"upload"]) -> None: ...
 
 global___InputsUpload = InputsUpload
+
+@typing_extensions.final
+class BookmarkOrigin(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _BookmarkType:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _BookmarkTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[BookmarkOrigin._BookmarkType.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        unknown: BookmarkOrigin._BookmarkType.ValueType  # 0
+        model: BookmarkOrigin._BookmarkType.ValueType  # 1
+        workflow: BookmarkOrigin._BookmarkType.ValueType  # 2
+        dataset: BookmarkOrigin._BookmarkType.ValueType  # 3
+        module: BookmarkOrigin._BookmarkType.ValueType  # 4
+
+    class BookmarkType(_BookmarkType, metaclass=_BookmarkTypeEnumTypeWrapper): ...
+    unknown: BookmarkOrigin.BookmarkType.ValueType  # 0
+    model: BookmarkOrigin.BookmarkType.ValueType  # 1
+    workflow: BookmarkOrigin.BookmarkType.ValueType  # 2
+    dataset: BookmarkOrigin.BookmarkType.ValueType  # 3
+    module: BookmarkOrigin.BookmarkType.ValueType  # 4
+
+    ID_FIELD_NUMBER: builtins.int
+    APP_ID_FIELD_NUMBER: builtins.int
+    USER_ID_FIELD_NUMBER: builtins.int
+    RESOURCE_TYPE_FIELD_NUMBER: builtins.int
+    id: builtins.str
+    """original resource id"""
+    app_id: builtins.str
+    """original resource app id"""
+    user_id: builtins.str
+    """original resource user id"""
+    resource_type: global___BookmarkOrigin.BookmarkType.ValueType
+    """resource type."""
+    def __init__(
+        self,
+        *,
+        id: builtins.str = ...,
+        app_id: builtins.str = ...,
+        user_id: builtins.str = ...,
+        resource_type: global___BookmarkOrigin.BookmarkType.ValueType = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["app_id", b"app_id", "id", b"id", "resource_type", b"resource_type", "user_id", b"user_id"]) -> None: ...
+
+global___BookmarkOrigin = BookmarkOrigin
+
+@typing_extensions.final
+class Runner(google.protobuf.message.Message):
+    """An app module that a user created in our app module marketplace."""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ID_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    CREATED_AT_FIELD_NUMBER: builtins.int
+    MODIFIED_AT_FIELD_NUMBER: builtins.int
+    METADATA_FIELD_NUMBER: builtins.int
+    USER_ID_FIELD_NUMBER: builtins.int
+    LABELS_FIELD_NUMBER: builtins.int
+    id: builtins.str
+    """A unique ID for this app module."""
+    description: builtins.str
+    """A short description for this app module to be used in grids of modules."""
+    @property
+    def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
+        """When the app module was created."""
+    @property
+    def modified_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
+        """When the app module was last modified."""
+    @property
+    def metadata(self) -> google.protobuf.struct_pb2.Struct:
+        """To handle arbitrary json metadata you can use a struct field:
+        https://github.com/google/protobuf/blob/master/src/google/protobuf/struct.proto
+        This is an optional arg.
+        """
+    user_id: builtins.str
+    """The creator of the app module."""
+    @property
+    def labels(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Labels to match."""
+    def __init__(
+        self,
+        *,
+        id: builtins.str = ...,
+        description: builtins.str = ...,
+        created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        metadata: google.protobuf.struct_pb2.Struct | None = ...,
+        user_id: builtins.str = ...,
+        labels: collections.abc.Iterable[builtins.str] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "metadata", b"metadata", "modified_at", b"modified_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "description", b"description", "id", b"id", "labels", b"labels", "metadata", b"metadata", "modified_at", b"modified_at", "user_id", b"user_id"]) -> None: ...
+
+global___Runner = Runner
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from clarifai_grpc.grpc.api.status import status_code_pb2 as proto_dot_clarifai_dot_api_dot_status_dot_status__code__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n proto/clarifai/api/service.proto\x12\x0c\x63larifai.api\x1a\"proto/clarifai/api/resources.proto\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/auth/scope/scope.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\",\n\nPagination\x12\x0c\n\x04page\x18\x01 \x01(\r\x12\x10\n\x08per_page\x18\x02 \x01(\r\"p\n\x14GetAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rannotation_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb7\x02\n\x16ListAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\x12\x10\n\x08user_ids\x18\t \x03(\t\x12\x19\n\x11model_version_ids\x18\n \x03(\t\x12-\n\x08statuses\x18\x05 \x03(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14list_all_annotations\x18\x06 \x01(\x08\x12\x1b\n\x13return_model_output\x18\x0c \x01(\x08\x12\x0c\n\x04page\x18\x07 \x01(\r\x12\x10\n\x08per_page\x18\x08 \x01(\r\x12\x0f\n\x07task_id\x18\x0b \x01(\tJ\x04\x08\x04\x10\x05\"x\n\x16PostAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\"\xa7\x01\n\x17PatchAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x1c\n\x14\x64\x65lete_if_empty_data\x18\x04 \x01(\x08\"\xb9\x01\n\x1dPatchAnnotationsStatusRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0bstatus_code\x18\x02 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\x12\x10\n\x08user_ids\x18\x03 \x03(\t\x12\x0f\n\x07task_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\"v\n\x1ePatchAnnotationsStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08user_ids\x18\x02 \x03(\t\x12\x15\n\rupdated_count\x18\x03 \x01(\r\"s\n\x17\x44\x65leteAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12\x15\n\rannotation_id\x18\x03 \x01(\t\"k\n\x18\x44\x65leteAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"u\n\x18SingleAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12,\n\nannotation\x18\x02 \x01(\x0b\x32\x18.clarifai.api.Annotation\"{\n\x17MultiAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.AnnotationB\x04\x80\xb5\x18\x01\"[\n\rGetAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"\xa5\x02\n\x0fListAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x16\n\x0csort_by_name\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x10\n\x04name\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\tB\t\n\x07sort_by\"c\n\x0fPostAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\"C\n\x10\x44\x65leteAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\xb9\x01\n\x10PatchAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\xb7\x01\n\x0fPatchAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\x81\x01\n\x13PatchAppsIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\xa3\x01\n\x17PostAppsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tapp_query\x18\x02 \x01(\x0b\x32\x16.clarifai.api.AppQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"`\n\x11SingleAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\"f\n\x10MultiAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.AppB\x04\x80\xb5\x18\x01\"\x8b\x01\n\x18ListCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x16list_all_collaborators\x18\x02 \x01(\x08\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x18PostCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\"\x8f\x01\n\x19PatchCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"|\n\x1a\x44\x65leteCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x18\n\x10\x63ollaborator_ids\x18\x02 \x03(\t\x12\x13\n\x0buser_emails\x18\x03 \x03(\t\"\x82\x01\n\x1aMultiCollaboratorsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.CollaboratorB\x04\x80\xb5\x18\x01\"l\n\x19ListCollaborationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x85\x01\n\x1bMultiCollaborationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0e\x63ollaborations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.CollaborationB\x04\x80\xb5\x18\x01\".\n\x14GetStatusCodeRequest\x12\x16\n\x0estatus_code_id\x18\x01 \x01(\t\"\x18\n\x16ListStatusCodesRequest\"G\n\x18SingleStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"u\n\x17MultiStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08statuses\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.status.Status\"X\n\x11GetConceptRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\"f\n\x13ListConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x91\x01\n\x18ListModelConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xaf\x01\n\x1bPostConceptsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rconcept_query\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ConceptQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"o\n\x13PostConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\"\x80\x01\n\x14PatchConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"j\n\x17GetConceptCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x15SingleConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x63oncept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\"r\n\x14MultiConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.ConceptB\x04\x80\xb5\x18\x01\"\x82\x01\n\x19MultiConceptCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x63oncept_counts\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ConceptCountB\x04\x80\xb5\x18\x01\"\xb1\x01\n\x1bListConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x11\n\tpredicate\x18\x03 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\r\x12\x10\n\x08per_page\x18\x06 \x01(\r\"\x9c\x01\n\x1bPostConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_relations\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelation\"q\n\x1d\x44\x65leteConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"M\n\x1aListKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x85\x01\n\x1aPostKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraph\"\x8f\x01\n\x1dPostConceptMappingJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12=\n\x14\x63oncept_mapping_jobs\x18\x02 \x03(\x0b\x32\x1f.clarifai.api.ConceptMappingJob\"\x8b\x01\n\x1cMultiConceptRelationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_relations\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelationB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1bMultiKnowledgeGraphResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraphB\x04\x80\xb5\x18\x01\"Z\n\x1eMultiConceptMappingJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x02 \x03(\t\"r\n\x19GetConceptLanguageRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\x82\x01\n\x1bListConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\xad\x01\n\x1cPatchConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x9c\x01\n\x1bPostConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x85\x01\n\x1dSingleConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10\x63oncept_language\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x8b\x01\n\x1cMultiConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_languages\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguageB\x04\x80\xb5\x18\x01\"T\n\x0fGetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"\\\n\x17GetVideoManifestRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"l\n\x16GetInputSamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9e\x01\n\x11ListInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x04 \x03(\t\"\x92\x01\n\x13StreamInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08per_page\x18\x02 \x01(\r\x12\x0f\n\x07last_id\x18\x03 \x01(\t\x12\x13\n\x0border_by_id\x18\x05 \x01(\x08\x12\x12\n\ndescending\x18\x04 \x01(\x08\"\xd3\x01\n\x11PostInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x19\n\x11inputs_add_job_id\x18\x03 \x01(\t\x12M\n\x1cinput_id_conflict_resolution\x18\x04 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"z\n\x12PatchInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"W\n\x12\x44\x65leteInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"Y\n\x13\x44\x65leteInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\tJ\x04\x08\x03\x10\x04\"f\n\x13SingleInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"]\n\x18GetVideoManifestResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0cmanifest_url\x18\x02 \x01(\t\"\xa0\x01\n\x12MultiInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.InputB\x04\x80\xb5\x18\x01\x12\x32\n\x0einputs_add_job\x18\x03 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"r\n\x1cMultiInputAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\"q\n\x18SingleInputCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x06\x63ounts\x18\x02 \x01(\x0b\x32\x18.clarifai.api.InputCount\"G\n\x14GetInputCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x97\x01\n\x13ListDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\"s\n\x11GetDatasetRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"o\n\x13PostDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\"\x80\x01\n\x14PatchDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"]\n\x15\x44\x65leteDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0b\x64\x61taset_ids\x18\x02 \x03(\t\"r\n\x14MultiDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.DatasetB\x04\x80\xb5\x18\x01\"l\n\x15SingleDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Dataset\"\x7f\n\x18ListDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"o\n\x16GetDatasetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb9\x01\n\x18PostDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x32\n\x0e\x64\x61taset_inputs\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.DatasetInput\x12$\n\x06search\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\"t\n\x1a\x44\x65leteDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"\xd2\x01\n\x19MultiDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x64\x61taset_inputs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.DatasetInputB\x04\x80\xb5\x18\x01\x12N\n\x1d\x64\x61taset_inputs_search_add_job\x18\x03 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"|\n\x1aSingleDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rdataset_input\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.DatasetInput\"\x81\x01\n\x1aListDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"{\n\x18GetDatasetVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\"\xa4\x02\n&ListDatasetVersionMetricsGroupsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\x12\x14\n\x0cparent_paths\x18\x06 \x03(\t\x12;\n\x05types\x18\x07 \x03(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12&\n\x06values\x18\x08 \x03(\x0b\x32\x16.google.protobuf.Value\"\x99\x01\n\x1aPostDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\"\xaa\x01\n\x1bPatchDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x1c\x44\x65leteDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61taset_version_ids\x18\x03 \x03(\t\"\xb7\x01\n\x1fPutDatasetVersionExportsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x33\n\x07\x65xports\x18\x04 \x03(\x0b\x32\".clarifai.api.DatasetVersionExport\"\x88\x01\n\x1bMultiDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10\x64\x61taset_versions\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersionB\x04\x80\xb5\x18\x01\"\x8b\x01\n!MultiDatasetVersionExportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x07\x65xports\x18\x02 \x03(\x0b\x32\".clarifai.api.DatasetVersionExportB\x04\x80\xb5\x18\x01\"\xae\x01\n\'MultiDatasetVersionMetricsGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12V\n\x1e\x64\x61taset_version_metrics_groups\x18\x02 \x03(\x0b\x32(.clarifai.api.DatasetVersionMetricsGroupB\x04\x80\xb5\x18\x01\"\x82\x01\n\x1cSingleDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x64\x61taset_version\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\"f\n#GetDatasetInputsSearchAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06job_id\x18\x02 \x01(\t\"\x8c\x01\n\'SingleDatasetInputsSearchAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x03job\x18\x02 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"\xb9\x01\n\x17PostModelOutputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12\"\n\x05model\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Model\"\x8f\x01\n\x16ListModelInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"P\n\rGetKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"\x9a\x01\n\x0fListKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x13\n\x0bnot_expired\x18\x04 \x01(\x08\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x11\n\tendpoints\x18\x06 \x03(\t\"e\n\x12ListAppKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"c\n\x0fPostKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\"S\n\x10\x44\x65leteKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"t\n\x10PatchKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"`\n\x11SingleKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03key\x18\x02 \x01(\x0b\x32\x11.clarifai.api.Key\"f\n\x10MultiKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.KeyB\x04\x80\xb5\x18\x01\"\xad\x01\n\x0fGetModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x16\n\x0etrained_before\x18\x05 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\"\xa3\x04\n\x11ListModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\n \x01(\x08\x12\x16\n\x0csort_by_name\x18\x0b \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\x0c \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\r \x01(\x08H\x00\x12\r\n\x05query\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x19\n\x11\x66ilter_by_user_id\x18\x16 \x01(\x08\x12\x15\n\rmodel_type_id\x18\x06 \x01(\t\x12\x14\n\x0ctrained_only\x18\x07 \x01(\x08\x12\x14\n\x0cinput_fields\x18\x08 \x03(\t\x12\x15\n\routput_fields\x18\t \x03(\t\x12\x0f\n\x07license\x18\x0f \x01(\t\x12\x15\n\rfeatured_only\x18\x10 \x01(\x08\x12\x14\n\x0cstarred_only\x18\x14 \x01(\x08\x12\x10\n\x08toolkits\x18\x11 \x03(\t\x12\x11\n\tuse_cases\x18\x12 \x03(\t\x12\x11\n\tlanguages\x18\x15 \x03(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\x12\x1c\n\x14\x64ont_fetch_from_main\x18\x17 \x01(\x08\x42\t\n\x07sort_byJ\x04\x08\x04\x10\x05\"K\n\x18GetResourceCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x8e\x01\n\x19GetResourceCountsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08\x64\x61tasets\x18\x02 \x01(\x03\x12\x0e\n\x06models\x18\x03 \x01(\x03\x12\x11\n\tworkflows\x18\x04 \x01(\x03\x12\x0f\n\x07modules\x18\x05 \x01(\x03\"\x80\x01\n\x19PatchModelToolkitsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08toolkits\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1ePatchModelCheckConsentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x16\n\x0e\x63heck_consents\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x19PatchModelUseCasesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08usecases\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x82\x01\n\x1aPatchModelLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x11\n\tlanguages\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"Z\n\x19MultiModelToolkitResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08toolkits\x18\x02 \x03(\t\"e\n\x1eMultiModelCheckConsentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x16\n\x0e\x63heck_consents\x18\x02 \x03(\t\"Z\n\x19MultiModelUseCaseResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08usecases\x18\x02 \x03(\t\"\\\n\x1aMultiModelLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x11\n\tlanguages\x18\x02 \x03(\t\"\x91\x01\n\x11PostModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ModelB\x02\x18\x01\x12#\n\x06models\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Model\"z\n\x12PatchModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Model\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\",\n\x0eIdUpdateSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06new_id\x18\x02 \x01(\t\"\x82\x01\n\x14PatchModelIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"W\n\x12\x44\x65leteModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\"g\n\x13\x44\x65leteModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\xa9\x01\n\x19PostModelsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0bmodel_query\x18\x02 \x01(\x0b\x32\x18.clarifai.api.ModelQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"f\n\x13SingleModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\"l\n\x12MultiModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.ModelB\x04\x80\xb5\x18\x01\"\xa2\x01\n\x19PatchModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"o\n\x16GetModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\"\xc5\x02\n\x18ListModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\x12\x13\n\x0b\x63oncept_ids\x18\x05 \x03(\t\x12\x14\n\x0ctrained_only\x18\x06 \x01(\x08\x12\x16\n\x0esort_ascending\x18\x07 \x01(\x08\x12\x1d\n\x13sort_by_status_code\x18\x08 \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\t \x01(\x08H\x00\x12\x1d\n\x13sort_by_description\x18\n \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\x0b \x01(\x08H\x00\x42\t\n\x07sort_by\"r\n\x19\x44\x65leteModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x12\n\nversion_id\x18\x04 \x01(\t\"|\n\x1aSingleModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rmodel_version\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\"\x82\x01\n\x19MultiModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0emodel_versions\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ModelVersionB\x04\x80\xb5\x18\x01\"\xef\x01\n\x18PostModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\t\x10\n\"\xb1\x01\n$PostWorkflowVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x43\n\x0cpublications\x18\x03 \x03(\x0b\x32-.clarifai.api.WorkflowVersionUnPublishRequest\"\xad\x01\n\"PostWorkflowVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x41\n\x0cpublications\x18\x03 \x03(\x0b\x32+.clarifai.api.WorkflowVersionPublishRequest\"3\n\x1dWorkflowVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"5\n\x1fWorkflowVersionUnPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"0\n\x1aModelVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa4\x01\n\x1fPostModelVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12>\n\x0cpublications\x18\x03 \x03(\x0b\x32(.clarifai.api.ModelVersionPublishRequest\"2\n\x1cModelVersionUnpublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa8\x01\n!PostModelVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12@\n\x0cpublications\x18\x03 \x03(\x0b\x32*.clarifai.api.ModelVersionUnpublishRequest\"z\n\x16PostEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"i\n\x16ListEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x89\x01\n\x14GetEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\revaluation_id\x18\x02 \x01(\t\x12)\n\x06\x66ields\x18\x03 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"\xb2\x01\n\"PostModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12/\n\x0c\x65val_metrics\x18\x04 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xa1\x01\n\"ListModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xc1\x01\n GetModelVersionEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x15\n\revaluation_id\x18\x04 \x01(\t\x12)\n\x06\x66ields\x18\x05 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"y\n\x19SingleEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\"x\n\x18MultiEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xd3\x01\n\x1ePostModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x0btest_search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05\"\xa1\x01\n\x1dGetModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"]\n\x13GetModelTypeRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rmodel_type_id\x18\x02 \x01(\t\"h\n\x15ListModelTypesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x1f\n\x1dListOpenSourceLicensesRequest\"_\n\x1eListOpenSourceLicensesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08licenses\x18\x02 \x03(\t\"y\n\x17SingleModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\nmodel_type\x18\x02 \x01(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\"\xf2\x01\n\x16MultiModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bmodel_types\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\x12\x35\n\x0fmodel_importers\x18\x03 \x01(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12@\n\x16triton_conda_envs_info\x18\x04 \x03(\x0b\x32 .clarifai.api.TritonCondaEnvInfo\"\x95\x01\n\"GetModelVersionInputExampleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x12\n\nexample_id\x18\x04 \x01(\t\"\xa3\x01\n$ListModelVersionInputExamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xa2\x01\n&SingleModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12K\n\x1bmodel_version_input_example\x18\x02 \x01(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\xa2\x01\n%MultiModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cmodel_version_input_examples\x18\x02 \x03(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\x7f\n\x1aListModelReferencesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x82\x01\n\x1bMultiModelReferenceResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10model_references\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.ModelReference\"o\n\x13MultiOutputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07outputs\x18\x02 \x03(\x0b\x32\x14.clarifai.api.OutputB\x04\x80\xb5\x18\x01\"V\n\x11ListScopesRequest\x12\x10\n\x08key_type\x18\x01 \x01(\t\x12/\n\x0buser_app_id\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"B\n\x0fMyScopesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"F\n\x13MyScopesUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x15\n\x13MyScopesRootRequest\"\xa5\x01\n\x16MultiScopeDepsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\nscope_deps\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ScopeDeps\x12\x31\n\rendpoint_deps\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.EndpointDeps\"\xa0\x01\n\x12MultiScopeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x1e\n\x03\x61pp\x18\x03 \x01(\x0b\x32\x11.clarifai.api.App\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeRootResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"O\n\x10GetSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x13ListSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\xc4\x01\n\x13PostSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05query\x18\x02 \x01(\x0b\x32\x13.clarifai.api.QueryB\x02\x18\x01\x12&\n\x08searches\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Pagination\"\x85\x01\n\x1aPatchInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x8a\x01\n\x1fPatchAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x7f\n\x14PatchSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x17PostSearchesByIDRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"R\n\x13\x44\x65leteSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xa7\x01\n\x1ePostAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"c\n$DeleteAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xb6\x01\n\x19PostInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\x12\x12\n\nonly_count\x18\x04 \x01(\x08\"i\n\x14SingleSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\"\xed\x01\n\x13MultiSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\x12\"\n\x05query\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Query\x12&\n\x08searches\x18\x05 \x03(\x0b\x32\x14.clarifai.api.Search\x12*\n\nhit_counts\x18\x06 \x03(\x0b\x32\x16.clarifai.api.HitCount\"\x94\x02\n\"PostAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12*\n\x0cground_truth\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\x12 \n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x35\n\x0f\x65valuation_type\x18\x06 \x01(\x0e\x32\x1c.clarifai.api.EvaluationType\"`\n!GetAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"U\n\"ListAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x9d\x01\n$MultiAnnotationSearchMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12H\n\x19\x61nnotation_search_metrics\x18\x02 \x03(\x0b\x32%.clarifai.api.AnnotationSearchMetrics\"o\n\x1cListAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"k\n\x1aGetAnnotationFilterRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1c\n\x14\x61nnotation_filter_id\x18\x02 \x01(\t\"\x8b\x01\n\x1cPostAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\x9c\x01\n\x1dPatchAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"p\n\x1e\x44\x65leteAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1d\n\x15\x61nnotation_filter_ids\x18\x02 \x03(\t\"\x8e\x01\n\x1dMultiAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilterB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1eSingleAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x11\x61nnotation_filter\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\\\n\x0eGetUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"c\n\x12SingleUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04user\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\"x\n\x1bPostValidatePasswordRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12(\n\x08password\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Password\"\x8e\x01\n SinglePasswordValidationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12=\n\x13password_violations\x18\x02 \x01(\x0b\x32 .clarifai.api.PasswordViolations\"\xbb\x01\n\x12GetWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x03 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x04 \x03(\t\x12\"\n\x1a\x65xclude_clarifai_workflows\x18\x05 \x01(\x08\"\xbb\x02\n\x14ListWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x14\n\nsort_by_id\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x0e\n\x02id\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\t\x12\x13\n\x0bsearch_term\x18\x0c \x01(\tB\t\n\x07sort_by\"r\n\x14PostWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\"\x83\x01\n\x15PatchWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x85\x01\n\x17PatchWorkflowIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\"j\n\x16\x44\x65leteWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"o\n\x16SingleWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\"u\n\x15MultiWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.WorkflowB\x04\x80\xb5\x18\x01\"\xa5\x02\n\x1aPostWorkflowResultsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12#\n\x06inputs\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\routput_config\x18\x04 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x05 \x01(\x08\x12\x33\n\x0eworkflow_state\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\xd8\x01\n\x1bPostWorkflowResultsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12-\n\x07results\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.WorkflowResult\x12\x33\n\x0eworkflow_state\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\x91\x02\n$PostWorkflowResultsSimilarityRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12)\n\x0cprobe_inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12(\n\x0bpool_inputs\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Input\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x06 \x01(\x08\"\x8e\x01\n%PostWorkflowResultsSimilarityResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x07results\x18\x02 \x03(\x0b\x32\'.clarifai.api.WorkflowResultsSimilarity\"\x83\x01\n\x1bListWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x19GetWorkflowVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x03 \x01(\t\"\x83\x01\n\x1d\x44\x65leteWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1c\n\x14workflow_version_ids\x18\x03 \x03(\t\"\xae\x01\n\x1cPatchWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x38\n\x11workflow_versions\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1cMultiWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11workflow_versions\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersionB\x04\x80\xb5\x18\x01\"\x85\x01\n\x1dSingleWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10workflow_version\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\"\x85\x01\n\x1aPostAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"g\n\x18GetAppDuplicationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1a\n\x12\x61pp_duplication_id\x18\x02 \x01(\t\"m\n\x1aListAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x83\x01\n\x1cMultiAppDuplicationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"\x82\x01\n\x1cSingleAppDuplicationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x61pp_duplication\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.AppDuplication\"f\n\x10PostTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\"m\n\x0eGetTaskRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\xee\x01\n\x10ListTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x17\n\x0fworker_user_ids\x18\x04 \x03(\t\x12\x17\n\x0freview_user_ids\x18\x05 \x03(\t\x12\x17\n\x0flabel_order_ids\x18\x08 \x03(\t\x12#\n\x1bincluding_label_order_tasks\x18\x06 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x07 \x03(\t\"w\n\x11PatchTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"R\n\x12\x44\x65leteTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x11MultiTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\'\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.TaskB\x04\x80\xb5\x18\x01\"c\n\x12SingleTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04task\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Task\"i\n\x13GetTaskCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9d\x01\n\x17SingleTaskCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0f\n\x07task_id\x18\x03 \x01(\t\x12\x34\n\x06\x63ounts\x18\x04 \x03(\x0b\x32$.clarifai.api.TaskStatusCountPerUser\"y\n\x16PostLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\"_\n\x14GetLabelOrderRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x16\n\x0elabel_order_id\x18\x02 \x01(\t\"i\n\x16ListLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x8a\x01\n\x17PatchLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"X\n\x18\x44\x65leteLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"|\n\x17MultiLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrderB\x04\x80\xb5\x18\x01\"v\n\x18SingleLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x0blabel_order\x18\x02 \x01(\x0b\x32\x18.clarifai.api.LabelOrder\"u\n\x15PostCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"\x86\x01\n\x16PatchCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"k\n\x17\x44\x65leteCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\\\n\x13GetCollectorRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x14\n\x0c\x63ollector_id\x18\x02 \x01(\t\"h\n\x15ListCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"r\n\x16MultiCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"r\n\x17SingleCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12*\n\tcollector\x18\x02 \x01(\x0b\x32\x17.clarifai.api.Collector\"v\n\x15PostStatValuesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12,\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValue\"y\n\x16MultiStatValueResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValueB\x04\x80\xb5\x18\x01\"\x9e\x01\n\x1ePostStatValuesAggregateRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12K\n\x1cstat_value_aggregate_queries\x18\x02 \x03(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"\x9c\x01\n\x1fMultiStatValueAggregateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cstat_value_aggregate_results\x18\x02 \x03(\x0b\x32&.clarifai.api.StatValueAggregateResult\"w\n\x1ePostTrendingMetricsViewRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\"\x85\x01\n\x1fListTrendingMetricsViewsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n MultiTrendingMetricsViewResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x07metrics\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.TrendingMetric\"q\n\x10GetModuleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\x96\x01\n\x12ListModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\"l\n\x12PostModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Module\"}\n\x13PatchModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Module\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"T\n\x14\x44\x65leteModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x14SingleModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06module\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Module\"o\n\x13MultiModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.ModuleB\x04\x80\xb5\x18\x01\"x\n\x17GetModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11module_version_id\x18\x03 \x01(\t\"\x7f\n\x19ListModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x95\x01\n\x19PostModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x34\n\x0fmodule_versions\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersion\"n\n\x1b\x44\x65leteModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"\x7f\n\x1bSingleModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\"\x85\x01\n\x1aMultiModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12:\n\x0fmodule_versions\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersionB\x04\x80\xb5\x18\x01\"x\n GetInstalledModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"u\n\"ListInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x9e\x01\n\"PostInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12G\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersion\"}\n%PostInstalledModuleVersionsKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"d\n$DeleteInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x9b\x01\n$SingleInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x46\n\x18installed_module_version\x18\x02 \x01(\x0b\x32$.clarifai.api.InstalledModuleVersion\"\xa1\x01\n#MultiInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12M\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersionB\x04\x80\xb5\x18\x01\"b\n\x1eListNextTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\x82\x01\n\x19PostBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0f\x62ulk_operations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"l\n\x19ListBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x17GetBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"Z\n\x1a\x43\x61ncelBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"Z\n\x1a\x44\x65leteBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x80\x01\n\x1cSingleBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.BulkOperation\"\x7f\n\x1bMultiBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"o\n\x19PutTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"k\n\x18ListInputsAddJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"U\n\x16GetInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"X\n\x19\x43\x61ncelInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\x83\x01\n\x19MultiInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0finputs_add_jobs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsAddJobB\x04\x80\xb5\x18\x01\"}\n\x1aSingleInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0einputs_add_job\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"l\n\x12PostUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"T\n\x14\x44\x65leteUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"e\n\x12ListUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x10GetUploadRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\"i\n\x14SingleUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06upload\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Upload\"i\n\x13MultiUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"\x9a\x01\n\x1cPutUploadContentPartsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\x12\x36\n\rcontent_parts\x18\x03 \x03(\x0b\x32\x1f.clarifai.api.UploadContentPart\"\xad\x01\n\x1cPostInputsDataSourcesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.InputsDataSource\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\"r\n\x1dGetInputsExtractionJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12 \n\x18inputs_extraction_job_id\x18\x02 \x01(\t\"r\n\x1fListInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x92\x01\n!SingleInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x15inputs_extraction_job\x18\x02 \x01(\x0b\x32!.clarifai.api.InputsExtractionJob\"\x92\x01\n MultiInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x41\n\x16inputs_extraction_jobs\x18\x02 \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\"a\n!CancelInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x7f\n\x18PostInputsUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x32\n\x0einputs_uploads\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsUpload*p\n\x1cOrganizationInvitationStatus\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x02\x12\r\n\tCANCELLED\x10\x03\x12\x0c\n\x08\x44\x45\x43LINED\x10\x04\x12\x0b\n\x07\x45XPIRED\x10\x05\x32\x8a\x83\x03\n\x02V2\x12\xae\x02\n\x14ListConceptRelations\x12).clarifai.api.ListConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"\xbe\x01\x82\xd3\xe4\x93\x02\xab\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x0b\x12\xe3\x01\n\x14PostConceptRelations\x12).clarifai.api.PostConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"t\x82\xd3\xe4\x93\x02^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xe2\x01\n\x16\x44\x65leteConceptRelations\x12+.clarifai.api.DeleteConceptRelationsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\r\x90\x9c\'\n\x90\x9c\'\x0b\x12\xe0\x01\n\x10GetConceptCounts\x12%.clarifai.api.GetConceptCountsRequest\x1a\'.clarifai.api.MultiConceptCountResponse\"|\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\x15\x12\x13/v2/concepts/status\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd5\x01\n\nGetConcept\x12\x1f.clarifai.api.GetConceptRequest\x1a#.clarifai.api.SingleConceptResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\x1b\x12\x19/v2/concepts/{concept_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xbd\x01\n\x0cListConcepts\x12!.clarifai.api.ListConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\x0e\x12\x0c/v2/concepts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xbd\x02\n\x11ListModelConcepts\x12&.clarifai.api.ListModelConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"\xdb\x01\x82\xd3\xe4\x93\x02\xc4\x01\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xee\x01\n\x14PostConceptsSearches\x12).clarifai.api.PostConceptsSearchesRequest\x1a\".clarifai.api.MultiConceptResponse\"\x86\x01\x82\xd3\xe4\x93\x02l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\x01*Z\x1a\"\x15/v2/concepts/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xc7\x01\n\x0cPostConcepts\x12!.clarifai.api.PostConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"p\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\"\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xc9\x01\n\rPatchConcepts\x12\".clarifai.api.PatchConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\x32\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x98\x02\n\x12GetConceptLanguage\x12\'.clarifai.api.GetConceptLanguageRequest\x1a+.clarifai.api.SingleConceptLanguageResponse\"\xab\x01\x82\xd3\xe4\x93\x02\x98\x01\x12\x64/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\x12./v2/concepts/{concept_id}/languages/{language}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\x85\x02\n\x14ListConceptLanguages\x12).clarifai.api.ListConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x82\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\x12#/v2/concepts/{concept_id}/languages\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\x8f\x02\n\x14PostConceptLanguages\x12).clarifai.api.PostConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9f\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(\"#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x91\x02\n\x15PatchConceptLanguages\x12*.clarifai.api.PatchConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9f\x01\x82\xd3\xe4\x93\x02\x88\x01\x32Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(2#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xf5\x01\n\x13ListKnowledgeGraphs\x12(.clarifai.api.ListKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\x1f\x12\x1d/v2/concepts/knowledge_graphs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xff\x01\n\x13PostKnowledgeGraphs\x12(.clarifai.api.PostKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x92\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\x01*Z\"\"\x1d/v2/concepts/knowledge_graphs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x82\x02\n\x16PostConceptMappingJobs\x12+.clarifai.api.PostConceptMappingJobsRequest\x1a,.clarifai.api.MultiConceptMappingJobResponse\"\x8c\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\x01*Z\x1f\"\x1a/v2/concepts/mappings/jobs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x97\x02\n\rGetAnnotation\x12\".clarifai.api.GetAnnotationRequest\x1a&.clarifai.api.SingleAnnotationResponse\"\xb9\x01\x82\xd3\xe4\x93\x02\x9e\x01\x12g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\x12\x31/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xd4\x01\n\x0fListAnnotations\x12$.clarifai.api.ListAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"t\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\x11\x12\x0f/v2/annotations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe7\x01\n\x0fPostAnnotations\x12$.clarifai.api.PostAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x86\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\"\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe9\x01\n\x10PatchAnnotations\x12%.clarifai.api.PatchAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x86\x01\x82\xd3\xe4\x93\x02`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\x32\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf8\x01\n\x16PatchAnnotationsStatus\x12+.clarifai.api.PatchAnnotationsStatusRequest\x1a,.clarifai.api.PatchAnnotationsStatusResponse\"\x82\x01\x82\xd3\xe4\x93\x02`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xa0\x02\n\x10\x44\x65leteAnnotation\x12%.clarifai.api.DeleteAnnotationRequest\x1a!.clarifai.api.status.BaseResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\x9e\x01*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd4\x02\n\x11\x44\x65leteAnnotations\x12&.clarifai.api.DeleteAnnotationsRequest\x1a!.clarifai.api.status.BaseResponse\"\xf3\x01\x82\xd3\xe4\x93\x02\xd0\x01*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\x01*Z\x1b*\x16/v2/inputs/annotations:\x01*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14*\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf7\x01\n\x18PatchAnnotationsSearches\x12-.clarifai.api.PatchAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x88\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\x32\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\x85\x02\n\x17PostAnnotationsSearches\x12,.clarifai.api.PostAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x98\x01\x82\xd3\xe4\x93\x02r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\"\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd5\x01\n\rGetInputCount\x12\".clarifai.api.GetInputCountRequest\x1a&.clarifai.api.SingleInputCountResponse\"x\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\x13\x12\x11/v2/inputs/status\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xcd\x01\n\x0cStreamInputs\x12!.clarifai.api.StreamInputsRequest\x1a .clarifai.api.MultiInputResponse\"x\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\x13\x12\x11/v2/inputs/stream\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x81\x02\n\x0fGetInputSamples\x12$.clarifai.api.GetInputSamplesRequest\x1a*.clarifai.api.MultiInputAnnotationResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\x12\"/v2/tasks/{task_id}/inputs/samples\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xcf\x01\n\x08GetInput\x12\x1d.clarifai.api.GetInputRequest\x1a!.clarifai.api.SingleInputResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17\x12\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x80\x02\n\x15GetInputVideoManifest\x12%.clarifai.api.GetVideoManifestRequest\x1a&.clarifai.api.GetVideoManifestResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/video_manifestZ&\x12$/v2/inputs/{input_id}/video_manifest\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xbb\x01\n\nListInputs\x12\x1f.clarifai.api.ListInputsRequest\x1a .clarifai.api.MultiInputResponse\"j\x82\xd3\xe4\x93\x02P\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\x0c\x12\n/v2/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd6\x01\n\nPostInputs\x12\x1f.clarifai.api.PostInputsRequest\x1a .clarifai.api.MultiInputResponse\"\x84\x01\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\"\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xcf\x01\n\x0bPatchInputs\x12 .clarifai.api.PatchInputsRequest\x1a .clarifai.api.MultiInputResponse\"|\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\x32\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x12\xe9\x01\n\x0b\x44\x65leteInput\x12 .clarifai.api.DeleteInputRequest\x1a!.clarifai.api.status.BaseResponse\"\x94\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17*\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xdb\x01\n\x0c\x44\x65leteInputs\x12!.clarifai.api.DeleteInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f*\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe2\x01\n\x13PatchInputsSearches\x12(.clarifai.api.PatchInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"~\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\x32\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\xf1\x01\n\x12PostInputsSearches\x12\'.clarifai.api.PostInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x8e\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\"\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xa0\x03\n\x10PostModelOutputs\x12%.clarifai.api.PostModelOutputsRequest\x1a!.clarifai.api.MultiOutputResponse\"\xc1\x02\x82\xd3\xe4\x93\x02\xa6\x02\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\x01*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\x01*Z\"\"\x1d/v2/models/{model_id}/outputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x02\x12\xef\x01\n\x0cListDatasets\x12!.clarifai.api.ListDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ*\x12(/v2/users/{user_app_id.user_id}/datasetsZ\x0e\x12\x0c/v2/datasets\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xd9\x01\n\nGetDataset\x12\x1f.clarifai.api.GetDatasetRequest\x1a#.clarifai.api.SingleDatasetResponse\"\x84\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\x1b\x12\x19/v2/datasets/{dataset_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xcb\x01\n\x0cPostDatasets\x12!.clarifai.api.PostDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"t\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\"\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xcd\x01\n\rPatchDatasets\x12\".clarifai.api.PatchDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"t\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\x32\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xce\x01\n\x0e\x44\x65leteDatasets\x12#.clarifai.api.DeleteDatasetsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11*\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\x81\x02\n\x11ListDatasetInputs\x12&.clarifai.api.ListDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\x9a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\x12 /v2/datasets/{dataset_id}/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x95\x02\n\x0fGetDatasetInput\x12$.clarifai.api.GetDatasetInputRequest\x1a(.clarifai.api.SingleDatasetInputResponse\"\xb1\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\x12+/v2/datasets/{dataset_id}/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x8c\x02\n\x11PostDatasetInputs\x12&.clarifai.api.PostDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%\" /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x86\x02\n\x13\x44\x65leteDatasetInputs\x12(.clarifai.api.DeleteDatasetInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x82\x01*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%* /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x90\x9c\'\x05\x12\x84\x02\n\x13ListDatasetVersions\x12(.clarifai.api.ListDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\x12\"/v2/datasets/{dataset_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xab\x02\n\x11GetDatasetVersion\x12&.clarifai.api.GetDatasetVersionRequest\x1a*.clarifai.api.SingleDatasetVersionResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\xaa\x01\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\x12\x37/v2/datasets/{dataset_id}/versions/{dataset_version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xea\x02\n\x1fListDatasetVersionMetricsGroups\x12\x34.clarifai.api.ListDatasetVersionMetricsGroupsRequest\x1a\x35.clarifai.api.MultiDatasetVersionMetricsGroupResponse\"\xd9\x01\x82\xd3\xe4\x93\x02\xba\x01\x12u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\x12?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x92\x02\n\x13PostDatasetVersions\x12(.clarifai.api.PostDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x86\x01\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'\"\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x8c\x02\n\x14PatchDatasetVersions\x12).clarifai.api.PatchDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01\x32X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'2\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x12\x8a\x02\n\x15\x44\x65leteDatasetVersions\x12*.clarifai.api.DeleteDatasetVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'*\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xd4\x02\n\x18PutDatasetVersionExports\x12-.clarifai.api.PutDatasetVersionExportsRequest\x1a/.clarifai.api.MultiDatasetVersionExportResponse\"\xd7\x01\x82\xd3\xe4\x93\x02\xc0\x01\x1au/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*ZD\x1a?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x12\xe9\x01\n\x0cGetModelType\x12!.clarifai.api.GetModelTypeRequest\x1a%.clarifai.api.SingleModelTypeResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\x12 /v2/models/types/{model_type_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\x99\x01\n\x16ListOpenSourceLicenses\x12+.clarifai.api.ListOpenSourceLicensesRequest\x1a,.clarifai.api.ListOpenSourceLicensesResponse\"$\x82\xd3\xe4\x93\x02\x1a\x12\x18/v2/open_source_licenses\x98\x9c\'\x01\x12\xcb\x01\n\x0eListModelTypes\x12#.clarifai.api.ListModelTypesRequest\x1a$.clarifai.api.MultiModelTypeResponse\"n\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\x12\x12\x10/v2/models/types\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xca\x01\n\x08GetModel\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"|\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17\x12\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\x9a\x03\n\x12GetModelOutputInfo\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"\xc1\x02\x82\xd3\xe4\x93\x02\xaa\x02\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\x12!/v2/models/{model_id}/output_infoZo\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\x12\x37/v2/models/{model_id}/versions/{version_id}/output_info\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe2\x01\n\nListModels\x12\x1f.clarifai.api.ListModelsRequest\x1a .clarifai.api.MultiModelResponse\"\x90\x01\x82\xd3\xe4\x93\x02z\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\x12&/v2/users/{user_app_id.user_id}/modelsZ\x0c\x12\n/v2/models\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe7\x01\n\x11GetResourceCounts\x12&.clarifai.api.GetResourceCountsRequest\x1a\'.clarifai.api.GetResourceCountsResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/resource_countsZ\x15\x12\x13/v2/resource_counts\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'m\x90\x9c\'-\x12\xdf\x01\n\x12PostModelsSearches\x12\'.clarifai.api.PostModelsSearchesRequest\x1a .clarifai.api.MultiModelResponse\"~\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\x01*Z\x18\"\x13/v2/models/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xca\x01\n\nPostModels\x12\x1f.clarifai.api.PostModelsRequest\x1a!.clarifai.api.SingleModelResponse\"x\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\"\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x12\xc7\x01\n\x0bPatchModels\x12 .clarifai.api.PatchModelsRequest\x1a .clarifai.api.MultiModelResponse\"t\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\x32\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x12\xb6\x01\n\rPatchModelIds\x12\".clarifai.api.PatchModelIdsRequest\x1a .clarifai.api.MultiModelResponse\"_\x82\xd3\xe4\x93\x02I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0e\x90\x9c\'\x0f\x12\xdd\x01\n\x0b\x44\x65leteModel\x12 .clarifai.api.DeleteModelRequest\x1a!.clarifai.api.status.BaseResponse\"\x88\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17*\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xce\x01\n\x0c\x44\x65leteModels\x12!.clarifai.api.DeleteModelsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f*\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x95\x02\n\x17PatchModelCheckConsents\x12,.clarifai.api.PatchModelCheckConsentsRequest\x1a,.clarifai.api.MultiModelCheckConsentResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\x01*Z)2$/v2/models/{model_id}/check_consents:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf9\x01\n\x12PatchModelToolkits\x12\'.clarifai.api.PatchModelToolkitsRequest\x1a\'.clarifai.api.MultiModelToolkitResponse\"\x90\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\x01*Z#2\x1e/v2/models/{model_id}/toolkits:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf9\x01\n\x12PatchModelUseCases\x12\'.clarifai.api.PatchModelUseCasesRequest\x1a\'.clarifai.api.MultiModelUseCaseResponse\"\x90\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\x01*Z#2\x1e/v2/models/{model_id}/usecases:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xff\x01\n\x13PatchModelLanguages\x12(.clarifai.api.PatchModelLanguagesRequest\x1a(.clarifai.api.MultiModelLanguageResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x80\x01\x32U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\x01*Z$2\x1f/v2/models/{model_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\x91\x03\n\x0fListModelInputs\x12$.clarifai.api.ListModelInputsRequest\x1a .clarifai.api.MultiInputResponse\"\xb5\x02\x82\xd3\xe4\x93\x02\x96\x02\x12R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\x1e\x12\x1c/v2/models/{model_id}/inputsZj\x12h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\x12\x32/v2/models/{model_id}/versions/{version_id}/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x12\x8d\x02\n\x0fGetModelVersion\x12$.clarifai.api.GetModelVersionRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\x12+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xf5\x01\n\x11ListModelVersions\x12&.clarifai.api.ListModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"\x8e\x01\x82\xd3\xe4\x93\x02x\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \x12\x1e/v2/models/{model_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xbc\x02\n\x1dPostWorkflowVersionsUnPublish\x12\x32.clarifai.api.PostWorkflowVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xc3\x01\x82\xd3\xe4\x93\x02\x8c\x01\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\x01*Z*\"%/v2/workflows/{workflow_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'x\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xb4\x02\n\x1bPostWorkflowVersionsPublish\x12\x30.clarifai.api.PostWorkflowVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbf\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\x01*Z(\"#/v2/workflows/{workflow_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'w\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xa1\x02\n\x18PostModelVersionsPublish\x12-.clarifai.api.PostModelVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb2\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\x01*Z\"\"\x1d/v2/models/{model_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'u\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xaa\x02\n\x1aPostModelVersionsUnPublish\x12/.clarifai.api.PostModelVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb7\x01\x82\xd3\xe4\x93\x02\x80\x01\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\x01*Z$\"\x1f/v2/models/{model_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'v\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x91\x02\n\x11PostModelVersions\x12&.clarifai.api.PostModelVersionsRequest\x1a!.clarifai.api.SingleModelResponse\"\xb0\x01\x82\xd3\xe4\x93\x02~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*Z#\"\x1e/v2/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdf\x01\n\x12PatchModelVersions\x12\'.clarifai.api.PatchModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"w\x82\xd3\xe4\x93\x02Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x0e\x90\x9c\'\x1a\x12\x98\x02\n\x12\x44\x65leteModelVersion\x12\'.clarifai.api.DeleteModelVersionRequest\x1a!.clarifai.api.status.BaseResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\x92\x01*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb7\x02\n\x16GetModelVersionMetrics\x12+.clarifai.api.GetModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xc5\x01\x82\xd3\xe4\x93\x02\xa2\x01\x12i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\x12\x33/v2/models/{model_id}/versions/{version_id}/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xd3\x02\n\x17PostModelVersionMetrics\x12,.clarifai.api.PostModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xdf\x01\x82\xd3\xe4\x93\x02\xa8\x01\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xed\x02\n\x1bPostModelVersionEvaluations\x12\x30.clarifai.api.PostModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xf3\x01\x82\xd3\xe4\x93\x02\xbc\x01\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\x01*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xd3\x02\n\x1bListModelVersionEvaluations\x12\x30.clarifai.api.ListModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xd9\x01\x82\xd3\xe4\x93\x02\xb6\x01\x12s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\x12=/v2/models/{model_id}/versions/{model_version_id}/evaluations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf1\x02\n\x19GetModelVersionEvaluation\x12..clarifai.api.GetModelVersionEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\xfa\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf8\x01\n\x0fPostEvaluations\x12$.clarifai.api.PostEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\x96\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations:\x01*Z\x14\"\x0f/v2/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdd\x01\n\x0fListEvaluations\x12$.clarifai.api.ListEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"|\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluationsZ\x11\x12\x0f/v2/evaluations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xfb\x01\n\rGetEvaluation\x12\".clarifai.api.GetEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations/{evaluation_id}Z!\x12\x1f/v2/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xfb\x01\n\x13ListModelReferences\x12(.clarifai.api.ListModelReferencesRequest\x1a).clarifai.api.MultiModelReferenceResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\x12 /v2/models/{model_id}/references\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf2\x02\n\x1bGetModelVersionInputExample\x12\x30.clarifai.api.GetModelVersionInputExampleRequest\x1a\x34.clarifai.api.SingleModelVersionInputExampleResponse\"\xea\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xda\x02\n\x1dListModelVersionInputExamples\x12\x32.clarifai.api.ListModelVersionInputExamplesRequest\x1a\x33.clarifai.api.MultiModelVersionInputExampleResponse\"\xcf\x01\x82\xd3\xe4\x93\x02\xbc\x01\x12v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\x12@/v2/models/{model_id}/versions/{model_version_id}/input_examples\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xe0\x01\n\x0bGetWorkflow\x12 .clarifai.api.GetWorkflowRequest\x1a$.clarifai.api.SingleWorkflowResponse\"\x88\x01\x82\xd3\xe4\x93\x02r\x12Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d\x12\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xf5\x01\n\rListWorkflows\x12\".clarifai.api.ListWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"\x9a\x01\x82\xd3\xe4\x93\x02\x83\x01\x12\x43/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\x12)/v2/users/{user_app_id.user_id}/workflowsZ\x0f\x12\r/v2/workflows\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xd0\x01\n\rPostWorkflows\x12\".clarifai.api.PostWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"v\x82\xd3\xe4\x93\x02\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\"\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xd2\x01\n\x0ePatchWorkflows\x12#.clarifai.api.PatchWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"v\x82\xd3\xe4\x93\x02\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\x32\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xc2\x01\n\x10PatchWorkflowIds\x12%.clarifai.api.PatchWorkflowIdsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"b\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x13\x12\xe7\x01\n\x0e\x44\x65leteWorkflow\x12#.clarifai.api.DeleteWorkflowRequest\x1a!.clarifai.api.status.BaseResponse\"\x8c\x01\x82\xd3\xe4\x93\x02r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d*\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\xd2\x01\n\x0f\x44\x65leteWorkflows\x12$.clarifai.api.DeleteWorkflowsRequest\x1a!.clarifai.api.status.BaseResponse\"v\x82\xd3\xe4\x93\x02\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12*\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\x8a\x03\n\x13PostWorkflowResults\x12(.clarifai.api.PostWorkflowResultsRequest\x1a).clarifai.api.PostWorkflowResultsResponse\"\x9d\x02\x82\xd3\xe4\x93\x02\xfe\x01\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\x01*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\x01*Z(\"#/v2/workflows/{workflow_id}/results:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\xc9\x03\n\x1dPostWorkflowResultsSimilarity\x12\x32.clarifai.api.PostWorkflowResultsSimilarityRequest\x1a\x33.clarifai.api.PostWorkflowResultsSimilarityResponse\"\xbe\x02\x82\xd3\xe4\x93\x02\x9f\x02\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\x01*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\x01*Z3\"./v2/workflows/{workflow_id}/results/similarity:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\x8b\x02\n\x14ListWorkflowVersions\x12).clarifai.api.ListWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\x12$/v2/workflows/{workflow_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb4\x02\n\x12GetWorkflowVersion\x12\'.clarifai.api.GetWorkflowVersionRequest\x1a+.clarifai.api.SingleWorkflowVersionResponse\"\xc7\x01\x82\xd3\xe4\x93\x02\xb0\x01\x12p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\x12:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x90\x02\n\x16\x44\x65leteWorkflowVersions\x12+.clarifai.api.DeleteWorkflowVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x8a\x01*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)*$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x13\x90\x9c\'\x12\x90\x9c\'\x15\x12\x97\x02\n\x15PatchWorkflowVersions\x12*.clarifai.api.PatchWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)2$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x85\x01\n\x06GetKey\x12\x1b.clarifai.api.GetKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"=\x82\xd3\xe4\x93\x02/\x12-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'0\x12\x7f\n\x08ListKeys\x12\x1d.clarifai.api.ListKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"4\x82\xd3\xe4\x93\x02&\x12$/v2/users/{user_app_id.user_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\xa3\x01\n\x0bListAppKeys\x12 .clarifai.api.ListAppKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"R\x82\xd3\xe4\x93\x02@\x12>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'0\x12\x95\x01\n\tDeleteKey\x12\x1e.clarifai.api.DeleteKeyRequest\x1a!.clarifai.api.status.BaseResponse\"E\x82\xd3\xe4\x93\x02/*-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'1\x90\x9c\'0\x12\x8a\x01\n\x08PostKeys\x12\x1d.clarifai.api.PostKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"?\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\x88\x01\n\tPatchKeys\x12\x1e.clarifai.api.PatchKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'0\x12\xbc\x01\n\x08MyScopes\x12\x1d.clarifai.api.MyScopesRequest\x1a .clarifai.api.MultiScopeResponse\"o\x82\xd3\xe4\x93\x02\x65\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/myscopesZ\x0e\x12\x0c/v2/myscopesZ\x0f\x12\r/v2/my_scopes\x98\x9c\'\x02\x12\x8d\x01\n\x0cMyScopesUser\x12!.clarifai.api.MyScopesUserRequest\x1a$.clarifai.api.MultiScopeUserResponse\"4\x82\xd3\xe4\x93\x02*\x12(/v2/users/{user_app_id.user_id}/myscopes\x98\x9c\'\x05\x12u\n\x0cMyScopesRoot\x12!.clarifai.api.MyScopesRootRequest\x1a$.clarifai.api.MultiScopeRootResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/myscopesroot\x98\x9c\'\x05\x12\x87\x01\n\nListScopes\x12\x1f.clarifai.api.ListScopesRequest\x1a$.clarifai.api.MultiScopeDepsResponse\"2\x82\xd3\xe4\x93\x02(\x12&/v2/users/{user_app_id.user_id}/scopes\x98\x9c\'\x03\x12\x95\x01\n\x06GetApp\x12\x1b.clarifai.api.GetAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"M\x82\xd3\xe4\x93\x02;\x12\x39/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\x8f\x01\n\x08ListApps\x12\x1d.clarifai.api.ListAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\x12$/v2/users/{user_app_id.user_id}/appsZ\n\x12\x08/v2/apps\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\xa5\x01\n\tDeleteApp\x12\x1e.clarifai.api.DeleteAppRequest\x1a!.clarifai.api.status.BaseResponse\"U\x82\xd3\xe4\x93\x02;*9/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'.\x90\x9c\'-\x90\x9c\'\x13\x12\x92\x01\n\x08PostApps\x12\x1d.clarifai.api.PostAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"G\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x88\x01\n\tPatchApps\x12\x1e.clarifai.api.PatchAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x92\x01\n\x0cPatchAppsIds\x12!.clarifai.api.PatchAppsIdsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"?\x82\xd3\xe4\x93\x02-2(/v2/users/{user_app_id.user_id}/apps/ids:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9c\x01\n\x08PatchApp\x12\x1d.clarifai.api.PatchAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"P\x82\xd3\xe4\x93\x02>29/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9f\x01\n\x10PostAppsSearches\x12%.clarifai.api.PostAppsSearchesRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\"-/v2/users/{user_app_id.user_id}/apps/searches:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12v\n\x07GetUser\x12\x1c.clarifai.api.GetUserRequest\x1a .clarifai.api.SingleUserResponse\"+\x82\xd3\xe4\x93\x02!\x12\x1f/v2/users/{user_app_id.user_id}\x98\x9c\'\x05\x12\xcf\x01\n\x14PostValidatePassword\x12).clarifai.api.PostValidatePasswordRequest\x1a..clarifai.api.SinglePasswordValidationResponse\"\\\x82\xd3\xe4\x93\x02R\"1/v2/users/{user_app_id.user_id}/validate_password:\x01*Z\x1a\"\x15/v2/validate_password:\x01*\x98\x9c\'\x03\x12\xc1\x01\n\tGetSearch\x12\x1e.clarifai.api.GetSearchRequest\x1a\".clarifai.api.SingleSearchResponse\"p\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13\x12\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xbc\x01\n\x0cListSearches\x12!.clarifai.api.ListSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\x0e\x12\x0c/v2/searches\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xc8\x01\n\rPatchSearches\x12\".clarifai.api.PatchSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\x32\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\xda\x01\n\x0cPostSearches\x12!.clarifai.api.PostSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x83\x01\x88\x02\x01\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\"\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd8\x01\n\x10PostSearchesByID\x12%.clarifai.api.PostSearchesByIDRequest\x1a!.clarifai.api.MultiSearchResponse\"z\x82\xd3\xe4\x93\x02\x64\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\x01*Z\x16\"\x11/v2/searches/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'\x03\x12\xb3\x02\n\x1bPostAnnotationSearchMetrics\x12\x30.clarifai.api.PostAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xad\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\x01*Z%\" /v2/annotations/searches/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x90\x9c\'6\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xa9\x02\n\x1aGetAnnotationSearchMetrics\x12/.clarifai.api.GetAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\x12%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\xa0\x02\n\x1bListAnnotationSearchMetrics\x12\x30.clarifai.api.ListAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\x9a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\x12 /v2/annotations/searches/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x9a\x02\n\x1d\x44\x65leteAnnotationSearchMetrics\x12\x32.clarifai.api.DeleteAnnotationSearchMetricsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'5\x90\x9c\'6\x90\x9c\'?\x12\xce\x01\n\x0c\x44\x65leteSearch\x12!.clarifai.api.DeleteSearchRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13*\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x90\x9c\'t\x12\xec\x01\n\x15ListAnnotationFilters\x12*.clarifai.api.ListAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"z\x82\xd3\xe4\x93\x02h\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\x18\x12\x16/v2/annotation_filters\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\x99\x02\n\x13GetAnnotationFilter\x12(.clarifai.api.GetAnnotationFilterRequest\x1a,.clarifai.api.SingleAnnotationFilterResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x96\x01\x12\x63/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\x12-/v2/annotation_filters/{annotation_filter_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xf7\x01\n\x15PostAnnotationFilters\x12*.clarifai.api.PostAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x84\x01\x82\xd3\xe4\x93\x02n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\"\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12\xf9\x01\n\x16PatchAnnotationFilters\x12+.clarifai.api.PatchAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x84\x01\x82\xd3\xe4\x93\x02n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\x32\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12\xf1\x01\n\x17\x44\x65leteAnnotationFilters\x12,.clarifai.api.DeleteAnnotationFiltersRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b*\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12|\n\x0fListStatusCodes\x12$.clarifai.api.ListStatusCodesRequest\x1a%.clarifai.api.MultiStatusCodeResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/status_codes\x98\x9c\'\x01\x12\x8a\x01\n\rGetStatusCode\x12\".clarifai.api.GetStatusCodeRequest\x1a&.clarifai.api.SingleStatusCodeResponse\"-\x82\xd3\xe4\x93\x02#\x12!/v2/status_codes/{status_code_id}\x98\x9c\'\x01\x12\xc2\x01\n\x11ListCollaborators\x12&.clarifai.api.ListCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"[\x82\xd3\xe4\x93\x02I\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'2\x12\xc9\x01\n\x11PostCollaborators\x12&.clarifai.api.PostCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"b\x82\xd3\xe4\x93\x02L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x12\xcf\x01\n\x12PatchCollaborators\x12\'.clarifai.api.PatchCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"f\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x12\xd2\x01\n\x13\x44\x65leteCollaborators\x12(.clarifai.api.DeleteCollaboratorsRequest\x1a!.clarifai.api.status.BaseResponse\"n\x82\xd3\xe4\x93\x02L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x90\x9c\'7\x90\x9c\'8\x12\xa4\x01\n\x12ListCollaborations\x12\'.clarifai.api.ListCollaborationsRequest\x1a).clarifai.api.MultiCollaborationsResponse\":\x82\xd3\xe4\x93\x02\x30\x12./v2/users/{user_app_id.user_id}/collaborations\x98\x9c\'\x03\x12\xf3\x01\n\x13PostAppDuplications\x12(.clarifai.api.PostAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"\x85\x01\x82\xd3\xe4\x93\x02K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\n\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x12\x90\x9c\'\x13\x12\xa5\x01\n\x13ListAppDuplications\x12(.clarifai.api.ListAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"8\x82\xd3\xe4\x93\x02.\x12,/v2/users/{user_app_id.user_id}/duplications\x98\x9c\'\x05\x12\xb6\x01\n\x11GetAppDuplication\x12&.clarifai.api.GetAppDuplicationRequest\x1a*.clarifai.api.SingleAppDuplicationResponse\"M\x82\xd3\xe4\x93\x02\x43\x12\x41/v2/users/{user_app_id.user_id}/duplications/{app_duplication_id}\x98\x9c\'\x05\x12\xd9\x01\n\tPostTasks\x12\x1e.clarifai.api.PostTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x8a\x01\x82\xd3\xe4\x93\x02T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\"\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'\x03\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xfe\x01\n\x16GetTaskAnnotationCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\x12%/v2/tasks/{task_id}/annotations/count\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x12\xee\x01\n\x11GetTaskInputCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\x12 /v2/tasks/{task_id}/inputs/count\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x12\xd0\x01\n\x07GetTask\x12\x1c.clarifai.api.GetTaskRequest\x1a .clarifai.api.SingleTaskResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\x15\x12\x13/v2/tasks/{task_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xbe\x01\n\tListTasks\x12\x1e.clarifai.api.ListTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"p\x82\xd3\xe4\x93\x02N\x12?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\x0b\x12\t/v2/tasks\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd7\x01\n\nPatchTasks\x12\x1f.clarifai.api.PatchTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x86\x01\x82\xd3\xe4\x93\x02T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\x32\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xc2\x01\n\x0b\x44\x65leteTasks\x12 .clarifai.api.DeleteTasksRequest\x1a!.clarifai.api.status.BaseResponse\"n\x82\xd3\xe4\x93\x02T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e*\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xf5\x01\n\x0fPostLabelOrders\x12$.clarifai.api.PostLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x94\x01\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\"\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf6\x01\n\rGetLabelOrder\x12\".clarifai.api.GetLabelOrderRequest\x1a&.clarifai.api.SingleLabelOrderResponse\"\x98\x01\x82\xd3\xe4\x93\x02~\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\x12!/v2/label_orders/{label_order_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xd6\x01\n\x0fListLabelOrders\x12$.clarifai.api.ListLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"v\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\x12\x12\x10/v2/label_orders\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xeb\x01\n\x10PatchLabelOrders\x12%.clarifai.api.PatchLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x88\x01\x82\xd3\xe4\x93\x02\x62\x32\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\x32\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'D\x90\x9c\'\x0b\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xe5\x01\n\x11\x44\x65leteLabelOrders\x12&.clarifai.api.DeleteLabelOrdersRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15*\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'E\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x12\xf2\x01\n\x0ePostCollectors\x12#.clarifai.api.PostCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"\x94\x01\x82\xd3\xe4\x93\x02^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\"\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'%\x90\x9c\'&\x90\x9c\')\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xe3\x01\n\x0cGetCollector\x12!.clarifai.api.GetCollectorRequest\x1a%.clarifai.api.SingleCollectorResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\x1f\x12\x1d/v2/collectors/{collector_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'*\x12\xc7\x01\n\x0eListCollectors\x12#.clarifai.api.ListCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"j\x82\xd3\xe4\x93\x02X\x12\x44/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\x10\x12\x0e/v2/collectors\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'*\x12\xd3\x01\n\x0fPatchCollectors\x12$.clarifai.api.PatchCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"t\x82\xd3\xe4\x93\x02^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\x32\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\')\x90\x9c\'*\x12\xd6\x01\n\x10\x44\x65leteCollectors\x12%.clarifai.api.DeleteCollectorsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13*\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\')\x90\x9c\'+\x90\x9c\'*\x12\xc9\x01\n\x0ePostStatValues\x12#.clarifai.api.PostStatValuesRequest\x1a$.clarifai.api.MultiStatValueResponse\"l\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values:\x01*Z\x15\"\x10/v2/stats/values:\x01*\x98\x9c\'\x02\x12\xfd\x01\n\x17PostStatValuesAggregate\x12,.clarifai.api.PostStatValuesAggregateRequest\x1a-.clarifai.api.MultiStatValueAggregateResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\x01*Z\x1f\"\x1a/v2/stats/values/aggregate:\x01*\x98\x9c\'\x02\x90\x9c\'-\x12\xe3\x01\n\x17PostTrendingMetricsView\x12,.clarifai.api.PostTrendingMetricsViewRequest\x1a!.clarifai.api.status.BaseResponse\"w\x82\xd3\xe4\x93\x02m\"h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}/{object_id}:\x01*\x98\x9c\'\x02\x12\x8f\x02\n\x18ListTrendingMetricsViews\x12-.clarifai.api.ListTrendingMetricsViewsRequest\x1a..clarifai.api.MultiTrendingMetricsViewResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x88\x01\x12\\/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}Z(\x12&/v2/trending_metrics/views/{view_type}\x98\x9c\'\x02\x12\xb2\x01\n\tGetModule\x12\x1e.clarifai.api.GetModuleRequest\x1a\".clarifai.api.SingleModuleResponse\"a\x82\xd3\xe4\x93\x02O\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xe4\x01\n\x0bListModules\x12 .clarifai.api.ListModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\x8f\x01\x82\xd3\xe4\x93\x02}\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\x12\'/v2/users/{user_app_id.user_id}/modulesZ\r\x12\x0b/v2/modules\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xb0\x01\n\x0bPostModules\x12 .clarifai.api.PostModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\\\x82\xd3\xe4\x93\x02\x46\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xb2\x01\n\x0cPatchModules\x12!.clarifai.api.PatchModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\\\x82\xd3\xe4\x93\x02\x46\x32\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xd0\x01\n\rDeleteModules\x12\".clarifai.api.DeleteModulesRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02\x46*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x90\x9c\'p\x90\x9c\'o\x90\x9c\'q\x90\x9c\'1\x90\x9c\'0\x90\x9c\'/\x12\xe4\x01\n\x10GetModuleVersion\x12%.clarifai.api.GetModuleVersionRequest\x1a).clarifai.api.SingleModuleVersionResponse\"~\x82\xd3\xe4\x93\x02l\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions/{module_version_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xd3\x01\n\x12ListModuleVersions\x12\'.clarifai.api.ListModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"j\x82\xd3\xe4\x93\x02X\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xda\x01\n\x12PostModuleVersions\x12\'.clarifai.api.PostModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"q\x82\xd3\xe4\x93\x02[\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xf4\x01\n\x14\x44\x65leteModuleVersions\x12).clarifai.api.DeleteModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x8d\x01\x82\xd3\xe4\x93\x02[*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x90\x9c\'p\x90\x9c\'o\x90\x9c\'q\x90\x9c\'1\x90\x9c\'0\x90\x9c\'/\x12\x8f\x02\n\x19GetInstalledModuleVersion\x12..clarifai.api.GetInstalledModuleVersionRequest\x1a\x32.clarifai.api.SingleInstalledModuleVersionResponse\"\x8d\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf3\x01\n\x1bListInstalledModuleVersions\x12\x30.clarifai.api.ListInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"o\x82\xd3\xe4\x93\x02U\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf6\x01\n\x1bPostInstalledModuleVersions\x12\x30.clarifai.api.PostInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"r\x82\xd3\xe4\x93\x02X\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x12\xfb\x01\n\x1d\x44\x65leteInstalledModuleVersions\x12\x32.clarifai.api.DeleteInstalledModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x82\x01\x82\xd3\xe4\x93\x02X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x90\x9c\'o\x90\x9c\'p\x90\x9c\'q\x90\x9c\'1\x90\x9c\'/\x90\x9c\'0\x12\x95\x02\n\x1ePostInstalledModuleVersionsKey\x12\x33.clarifai.api.PostInstalledModuleVersionsKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\"u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}/key:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\xf5\x01\n\x12PostBulkOperations\x12\'.clarifai.api.PostBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\"\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x90\x9c\'y\x90\x9c\'%\x90\x9c\'&\x90\x9c\'(\x12\xde\x01\n\x12ListBulkOperations\x12\'.clarifai.api.ListBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"t\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\x15\x12\x13/v2/bulk_operations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x12\xe5\x01\n\x10GetBulkOperation\x12%.clarifai.api.GetBulkOperationRequest\x1a*.clarifai.api.SingleBulkOperationsResponse\"~\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\x1a\x12\x18/v2/bulk_operations/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x12\xeb\x01\n\x14\x43\x61ncelBulkOperations\x12(.clarifai.api.CancelBulkOperationRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"~\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\x32\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'y\x90\x9c\'z\x12\xf4\x01\n\x14\x44\x65leteBulkOperations\x12(.clarifai.api.DeleteBulkOperationRequest\x1a!.clarifai.api.status.BaseResponse\"\x8e\x01\x82\xd3\xe4\x93\x02h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18*\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'%\x90\x9c\'(\x90\x9c\'y\x90\x9c\'z\x90\x9c\'{\x12\xb2\x02\n\x1cGetDatasetInputsSearchAddJob\x12\x31.clarifai.api.GetDatasetInputsSearchAddJobRequest\x1a\x35.clarifai.api.SingleDatasetInputsSearchAddJobResponse\"\xa7\x01\x82\xd3\xe4\x93\x02\x94\x01\x12\x62/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\x12,/v2/datasets/inputs/search_add/jobs/{job_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x12\x88\x02\n\x17ListNextTaskAssignments\x12,.clarifai.api.ListNextTaskAssignmentsRequest\x1a .clarifai.api.MultiInputResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\x12\x1f/v2/tasks/{task_id}/assignments\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xe3\x01\n\x12PutTaskAssignments\x12\'.clarifai.api.PutTaskAssignmentsRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02Z\x1aU/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xda\x01\n\x11ListInputsAddJobs\x12&.clarifai.api.ListInputsAddJobsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"t\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\x15\x12\x13/v2/inputs/jobs/add\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xe1\x01\n\x0fGetInputsAddJob\x12$.clarifai.api.GetInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"~\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\x1a\x12\x18/v2/inputs/jobs/add/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xf2\x01\n\x12\x43\x61ncelInputsAddJob\x12\'.clarifai.api.CancelInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}:\x01*Z\x1d\x32\x18/v2/inputs/jobs/add/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'\x05\x12\xc4\x01\n\x0bPostUploads\x12 .clarifai.api.PostUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"p\x82\xd3\xe4\x93\x02X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10\"\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\x8c\x02\n\x15PutUploadContentParts\x12*.clarifai.api.PutUploadContentPartsRequest\x1a\".clarifai.api.SingleUploadResponse\"\xa2\x01\x82\xd3\xe4\x93\x02\x89\x01\x1a[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\x01*Z\'\x1a%/v2/uploads/{upload_id}/content_parts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\xce\x01\n\tGetUpload\x12\x1e.clarifai.api.GetUploadRequest\x1a\".clarifai.api.SingleUploadResponse\"}\x82\xd3\xe4\x93\x02j\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\x19\x12\x17/v2/uploads/{upload_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x12\xb9\x01\n\x0bListUploads\x12 .clarifai.api.ListUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"e\x82\xd3\xe4\x93\x02R\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\x12\x0b/v2/uploads\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x12\xcd\x01\n\rDeleteUploads\x12\".clarifai.api.DeleteUploadsRequest\x1a!.clarifai.api.status.BaseResponse\"u\x82\xd3\xe4\x93\x02X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10*\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x90\x9c\'\x81\x01\x90\x9c\'\x82\x01\x12\x8d\x02\n\x15PostInputsDataSources\x12*.clarifai.api.PostInputsDataSourcesRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9e\x01\x82\xd3\xe4\x93\x02p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\x01*Z\x1c\"\x17/v2/inputs/data_sources:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xb2\x02\n\x16GetInputsExtractionJob\x12+.clarifai.api.GetInputsExtractionJobRequest\x1a/.clarifai.api.SingleInputsExtractionJobResponse\"\xb9\x01\x82\xd3\xe4\x93\x02\xa6\x01\x12k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\x12\x35/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xfe\x01\n\x18ListInputsExtractionJobs\x12-.clarifai.api.ListInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x82\x01\x82\xd3\xe4\x93\x02p\x12P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\x1c\x12\x1a/v2/inputs/jobs/extraction\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\x8c\x02\n\x1a\x43\x61ncelInputsExtractionJobs\x12/.clarifai.api.CancelInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x8c\x01\x82\xd3\xe4\x93\x02v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\x01*Z\x1f\x32\x1a/v2/inputs/jobs/extraction:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'\x05\x12\x85\x02\n\x11PostInputsUploads\x12&.clarifai.api.PostInputsUploadsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9e\x01\x82\xd3\xe4\x93\x02\x66\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\x01*Z\x17\"\x12/v2/inputs/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n proto/clarifai/api/service.proto\x12\x0c\x63larifai.api\x1a\"proto/clarifai/api/resources.proto\x1a&proto/clarifai/api/status/status.proto\x1a)proto/clarifai/api/utils/extensions.proto\x1a%proto/clarifai/auth/scope/scope.proto\x1a(proto/clarifai/auth/util/extension.proto\x1a+proto/clarifai/api/status/status_code.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\",\n\nPagination\x12\x0c\n\x04page\x18\x01 \x01(\r\x12\x10\n\x08per_page\x18\x02 \x01(\r\"p\n\x14GetAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rannotation_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb7\x02\n\x16ListAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\x12\x10\n\x08user_ids\x18\t \x03(\t\x12\x19\n\x11model_version_ids\x18\n \x03(\t\x12-\n\x08statuses\x18\x05 \x03(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1c\n\x14list_all_annotations\x18\x06 \x01(\x08\x12\x1b\n\x13return_model_output\x18\x0c \x01(\x08\x12\x0c\n\x04page\x18\x07 \x01(\r\x12\x10\n\x08per_page\x18\x08 \x01(\r\x12\x0f\n\x07task_id\x18\x0b \x01(\tJ\x04\x08\x04\x10\x05\"x\n\x16PostAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\"\xa7\x01\n\x17PatchAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.Annotation\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x1c\n\x14\x64\x65lete_if_empty_data\x18\x04 \x01(\x08\"\xb9\x01\n\x1dPatchAnnotationsStatusRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0bstatus_code\x18\x02 \x01(\x0e\x32\x1f.clarifai.api.status.StatusCode\x12\x10\n\x08user_ids\x18\x03 \x03(\t\x12\x0f\n\x07task_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\"v\n\x1ePatchAnnotationsStatusResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08user_ids\x18\x02 \x03(\t\x12\x15\n\rupdated_count\x18\x03 \x01(\r\"s\n\x17\x44\x65leteAnnotationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\x12\x15\n\rannotation_id\x18\x03 \x01(\t\"k\n\x18\x44\x65leteAnnotationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"u\n\x18SingleAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12,\n\nannotation\x18\x02 \x01(\x0b\x32\x18.clarifai.api.Annotation\"{\n\x17MultiAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0b\x61nnotations\x18\x02 \x03(\x0b\x32\x18.clarifai.api.AnnotationB\x04\x80\xb5\x18\x01\"[\n\rGetAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"\xe1\x02\n\x0fListAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x16\n\x0csort_by_name\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\x0c \x01(\x08H\x00\x12\x1c\n\x12sort_by_star_count\x18\r \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x10\n\x04name\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\tB\t\n\x07sort_by\"c\n\x0fPostAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\"C\n\x10\x44\x65leteAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\xb9\x01\n\x10PatchAppsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\xb7\x01\n\x0fPatchAppRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x32\n\x0fmetadata_action\x18\x04 \x01(\x0b\x32\x19.clarifai.api.PatchAction\x12\x0f\n\x07reindex\x18\x05 \x01(\x08\"\x81\x01\n\x13PatchAppsIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\xa3\x01\n\x17PostAppsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tapp_query\x18\x02 \x01(\x0b\x32\x16.clarifai.api.AppQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"`\n\x11SingleAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03\x61pp\x18\x02 \x01(\x0b\x32\x11.clarifai.api.App\"f\n\x10MultiAppResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04\x61pps\x18\x02 \x03(\x0b\x32\x11.clarifai.api.AppB\x04\x80\xb5\x18\x01\"\x8b\x01\n\x18ListCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1e\n\x16list_all_collaborators\x18\x02 \x01(\x08\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x18PostCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\"\x8f\x01\n\x19PatchCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.Collaborator\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"|\n\x1a\x44\x65leteCollaboratorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x18\n\x10\x63ollaborator_ids\x18\x02 \x03(\t\x12\x13\n\x0buser_emails\x18\x03 \x03(\t\"\x82\x01\n\x1aMultiCollaboratorsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\rcollaborators\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.CollaboratorB\x04\x80\xb5\x18\x01\"l\n\x19ListCollaborationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x85\x01\n\x1bMultiCollaborationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0e\x63ollaborations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.CollaborationB\x04\x80\xb5\x18\x01\".\n\x14GetStatusCodeRequest\x12\x16\n\x0estatus_code_id\x18\x01 \x01(\t\"\x18\n\x16ListStatusCodesRequest\"G\n\x18SingleStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\"u\n\x17MultiStatusCodeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08statuses\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.status.Status\"X\n\x11GetConceptRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\"f\n\x13ListConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x91\x01\n\x18ListModelConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xaf\x01\n\x1bPostConceptsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x31\n\rconcept_query\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ConceptQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"o\n\x13PostConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\"\x80\x01\n\x14PatchConceptsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Concept\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"j\n\x17GetConceptCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x15SingleConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x63oncept\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Concept\"r\n\x14MultiConceptResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x15.clarifai.api.ConceptB\x04\x80\xb5\x18\x01\"\x82\x01\n\x19MultiConceptCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x63oncept_counts\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ConceptCountB\x04\x80\xb5\x18\x01\"\xb1\x01\n\x1bListConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x11\n\tpredicate\x18\x03 \x01(\t\x12\x1a\n\x12knowledge_graph_id\x18\x04 \x01(\t\x12\x0c\n\x04page\x18\x05 \x01(\r\x12\x10\n\x08per_page\x18\x06 \x01(\r\"\x9c\x01\n\x1bPostConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_relations\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelation\"q\n\x1d\x44\x65leteConceptRelationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"M\n\x1aListKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x85\x01\n\x1aPostKnowledgeGraphsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraph\"\x8f\x01\n\x1dPostConceptMappingJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12=\n\x14\x63oncept_mapping_jobs\x18\x02 \x03(\x0b\x32\x1f.clarifai.api.ConceptMappingJob\"\x8b\x01\n\x1cMultiConceptRelationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_relations\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptRelationB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1bMultiKnowledgeGraphResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10knowledge_graphs\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.KnowledgeGraphB\x04\x80\xb5\x18\x01\"Z\n\x1eMultiConceptMappingJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x02 \x03(\t\"r\n\x19GetConceptLanguageRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\x82\x01\n\x1bListConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\xad\x01\n\x1cPatchConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x9c\x01\n\x1bPostConceptLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\nconcept_id\x18\x02 \x01(\t\x12\x38\n\x11\x63oncept_languages\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x85\x01\n\x1dSingleConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10\x63oncept_language\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.ConceptLanguage\"\x8b\x01\n\x1cMultiConceptLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11\x63oncept_languages\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.ConceptLanguageB\x04\x80\xb5\x18\x01\"T\n\x0fGetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"\\\n\x17GetVideoManifestRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"l\n\x16GetInputSamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9e\x01\n\x11ListInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12+\n\x06status\x18\x05 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0b\n\x03ids\x18\x04 \x03(\t\"\x92\x01\n\x13StreamInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08per_page\x18\x02 \x01(\r\x12\x0f\n\x07last_id\x18\x03 \x01(\t\x12\x13\n\x0border_by_id\x18\x05 \x01(\x08\x12\x12\n\ndescending\x18\x04 \x01(\x08\"\xd3\x01\n\x11PostInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x19\n\x11inputs_add_job_id\x18\x03 \x01(\t\x12M\n\x1cinput_id_conflict_resolution\x18\x04 \x01(\x0e\x32\'.clarifai.api.InputIDConflictResolution\"z\n\x12PatchInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"W\n\x12\x44\x65leteInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08input_id\x18\x02 \x01(\t\"Y\n\x13\x44\x65leteInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\tJ\x04\x08\x03\x10\x04\"f\n\x13SingleInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05input\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Input\"]\n\x18GetVideoManifestResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x14\n\x0cmanifest_url\x18\x02 \x01(\t\"\xa0\x01\n\x12MultiInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x13.clarifai.api.InputB\x04\x80\xb5\x18\x01\x12\x32\n\x0einputs_add_job\x18\x03 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"r\n\x1cMultiInputAnnotationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\"q\n\x18SingleInputCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x06\x63ounts\x18\x02 \x01(\x0b\x32\x18.clarifai.api.InputCount\"G\n\x14GetInputCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\xa7\x02\n\x13ListDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\x12\x16\n\x0esort_ascending\x18\x06 \x01(\x08\x12\x1c\n\x12sort_by_created_at\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12sort_by_star_count\x18\x08 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\t \x01(\x08H\x00\x12\x10\n\x08\x62ookmark\x18\n \x01(\x08\x42\t\n\x07sort_by\"s\n\x11GetDatasetRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"o\n\x13PostDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\"\x80\x01\n\x14PatchDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\'\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.Dataset\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"]\n\x15\x44\x65leteDatasetsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0b\x64\x61taset_ids\x18\x02 \x03(\t\"r\n\x14MultiDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x08\x64\x61tasets\x18\x02 \x03(\x0b\x32\x15.clarifai.api.DatasetB\x04\x80\xb5\x18\x01\"l\n\x15SingleDatasetResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12&\n\x07\x64\x61taset\x18\x02 \x01(\x0b\x32\x15.clarifai.api.Dataset\"\x7f\n\x18ListDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"o\n\x16GetDatasetInputRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"\xb9\x01\n\x18PostDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x32\n\x0e\x64\x61taset_inputs\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.DatasetInput\x12$\n\x06search\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\"t\n\x1a\x44\x65leteDatasetInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x11\n\tinput_ids\x18\x03 \x03(\t\"\xd2\x01\n\x19MultiDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0e\x64\x61taset_inputs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.DatasetInputB\x04\x80\xb5\x18\x01\x12N\n\x1d\x64\x61taset_inputs_search_add_job\x18\x03 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"|\n\x1aSingleDatasetInputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rdataset_input\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.DatasetInput\"\x81\x01\n\x1aListDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"{\n\x18GetDatasetVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\"\xa4\x02\n&ListDatasetVersionMetricsGroupsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\x12\x14\n\x0cparent_paths\x18\x06 \x03(\t\x12;\n\x05types\x18\x07 \x03(\x0e\x32,.clarifai.api.DatasetVersionMetricsGroupType\x12&\n\x06values\x18\x08 \x03(\x0b\x32\x16.google.protobuf.Value\"\x99\x01\n\x1aPostDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\"\xaa\x01\n\x1bPatchDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x36\n\x10\x64\x61taset_versions\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x1c\x44\x65leteDatasetVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x61taset_version_ids\x18\x03 \x03(\t\"\xb7\x01\n\x1fPutDatasetVersionExportsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x12\n\ndataset_id\x18\x02 \x01(\t\x12\x1a\n\x12\x64\x61taset_version_id\x18\x03 \x01(\t\x12\x33\n\x07\x65xports\x18\x04 \x03(\x0b\x32\".clarifai.api.DatasetVersionExport\"\x88\x01\n\x1bMultiDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12<\n\x10\x64\x61taset_versions\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.DatasetVersionB\x04\x80\xb5\x18\x01\"\x8b\x01\n!MultiDatasetVersionExportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x07\x65xports\x18\x02 \x03(\x0b\x32\".clarifai.api.DatasetVersionExportB\x04\x80\xb5\x18\x01\"\xae\x01\n\'MultiDatasetVersionMetricsGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12V\n\x1e\x64\x61taset_version_metrics_groups\x18\x02 \x03(\x0b\x32(.clarifai.api.DatasetVersionMetricsGroupB\x04\x80\xb5\x18\x01\"\x82\x01\n\x1cSingleDatasetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x64\x61taset_version\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.DatasetVersion\"f\n#GetDatasetInputsSearchAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06job_id\x18\x02 \x01(\t\"\x8c\x01\n\'SingleDatasetInputsSearchAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x03job\x18\x02 \x01(\x0b\x32\'.clarifai.api.DatasetInputsSearchAddJob\"\xb9\x01\n\x17PostModelOutputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12\"\n\x05model\x18\x05 \x01(\x0b\x32\x13.clarifai.api.Model\"\x8f\x01\n\x16ListModelInputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"P\n\rGetKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"\x9a\x01\n\x0fListKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x13\n\x0bnot_expired\x18\x04 \x01(\x08\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x11\n\tendpoints\x18\x06 \x03(\t\"e\n\x12ListAppKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"c\n\x0fPostKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\"S\n\x10\x44\x65leteKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"t\n\x10PatchKeysRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1f\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.Key\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"`\n\x11SingleKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x1e\n\x03key\x18\x02 \x01(\x0b\x32\x11.clarifai.api.Key\"f\n\x10MultiKeyResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x04keys\x18\x02 \x03(\x0b\x32\x11.clarifai.api.KeyB\x04\x80\xb5\x18\x01\"\xad\x01\n\x0fGetModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\x12\x16\n\x0etrained_before\x18\x05 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\"\xf1\x04\n\x11ListModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\n \x01(\x08\x12\x16\n\x0csort_by_name\x18\x0b \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\x0c \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\r \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\x18 \x01(\x08H\x00\x12\x1c\n\x12sort_by_star_count\x18\x19 \x01(\x08H\x00\x12\r\n\x05query\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x19\n\x11\x66ilter_by_user_id\x18\x16 \x01(\x08\x12\x15\n\rmodel_type_id\x18\x06 \x01(\t\x12\x14\n\x0ctrained_only\x18\x07 \x01(\x08\x12\x14\n\x0cinput_fields\x18\x08 \x03(\t\x12\x15\n\routput_fields\x18\t \x03(\t\x12\x0f\n\x07license\x18\x0f \x01(\t\x12\x15\n\rfeatured_only\x18\x10 \x01(\x08\x12\x14\n\x0cstarred_only\x18\x14 \x01(\x08\x12\x10\n\x08toolkits\x18\x11 \x03(\t\x12\x11\n\tuse_cases\x18\x12 \x03(\t\x12\x11\n\tlanguages\x18\x15 \x03(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x13 \x03(\t\x12\x1c\n\x14\x64ont_fetch_from_main\x18\x17 \x01(\x08\x12\x10\n\x08\x62ookmark\x18\x1a \x01(\x08\x42\t\n\x07sort_byJ\x04\x08\x04\x10\x05\"K\n\x18GetResourceCountsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x8e\x01\n\x19GetResourceCountsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08\x64\x61tasets\x18\x02 \x01(\x03\x12\x0e\n\x06models\x18\x03 \x01(\x03\x12\x11\n\tworkflows\x18\x04 \x01(\x03\x12\x0f\n\x07modules\x18\x05 \x01(\x03\"\x80\x01\n\x19PatchModelToolkitsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08toolkits\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1ePatchModelCheckConsentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x16\n\x0e\x63heck_consents\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x80\x01\n\x19PatchModelUseCasesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08usecases\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x82\x01\n\x1aPatchModelLanguagesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x11\n\tlanguages\x18\x03 \x03(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"Z\n\x19MultiModelToolkitResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08toolkits\x18\x02 \x03(\t\"e\n\x1eMultiModelCheckConsentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x16\n\x0e\x63heck_consents\x18\x02 \x03(\t\"Z\n\x19MultiModelUseCaseResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08usecases\x18\x02 \x03(\t\"\\\n\x1aMultiModelLanguageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x11\n\tlanguages\x18\x02 \x03(\t\"\x91\x01\n\x11PostModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.ModelB\x02\x18\x01\x12#\n\x06models\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Model\"z\n\x12PatchModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.Model\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\",\n\x0eIdUpdateSource\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06new_id\x18\x02 \x01(\t\"\x82\x01\n\x14PatchModelIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"W\n\x12\x44\x65leteModelRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\"g\n\x13\x44\x65leteModelsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\xa9\x01\n\x19PostModelsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12-\n\x0bmodel_query\x18\x02 \x01(\x0b\x32\x18.clarifai.api.ModelQuery\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"f\n\x13SingleModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\"\n\x05model\x18\x02 \x01(\x0b\x32\x13.clarifai.api.Model\"l\n\x12MultiModelResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12)\n\x06models\x18\x02 \x03(\x0b\x32\x13.clarifai.api.ModelB\x04\x80\xb5\x18\x01\"\xa2\x01\n\x19PatchModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"o\n\x16GetModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\"\xc5\x02\n\x18ListModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\x12\x13\n\x0b\x63oncept_ids\x18\x05 \x03(\t\x12\x14\n\x0ctrained_only\x18\x06 \x01(\x08\x12\x16\n\x0esort_ascending\x18\x07 \x01(\x08\x12\x1d\n\x13sort_by_status_code\x18\x08 \x01(\x08H\x00\x12\x1c\n\x12sort_by_num_inputs\x18\t \x01(\x08H\x00\x12\x1d\n\x13sort_by_description\x18\n \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\x0b \x01(\x08H\x00\x42\t\n\x07sort_by\"r\n\x19\x44\x65leteModelVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x12\n\nversion_id\x18\x04 \x01(\t\"|\n\x1aSingleModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\rmodel_version\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.ModelVersion\"\x82\x01\n\x19MultiModelVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x0emodel_versions\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.ModelVersionB\x04\x80\xb5\x18\x01\"\xef\x01\n\x18PostModelVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x32\n\x0emodel_versions\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.ModelVersion\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\t\x10\n\"\xb1\x01\n$PostWorkflowVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x43\n\x0cpublications\x18\x03 \x03(\x0b\x32-.clarifai.api.WorkflowVersionUnPublishRequest\"\xad\x01\n\"PostWorkflowVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x41\n\x0cpublications\x18\x03 \x03(\x0b\x32+.clarifai.api.WorkflowVersionPublishRequest\"3\n\x1dWorkflowVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"5\n\x1fWorkflowVersionUnPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"0\n\x1aModelVersionPublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa4\x01\n\x1fPostModelVersionsPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12>\n\x0cpublications\x18\x03 \x03(\x0b\x32(.clarifai.api.ModelVersionPublishRequest\"2\n\x1cModelVersionUnpublishRequest\x12\x12\n\nversion_id\x18\x01 \x01(\t\"\xa8\x01\n!PostModelVersionsUnPublishRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12@\n\x0cpublications\x18\x03 \x03(\x0b\x32*.clarifai.api.ModelVersionUnpublishRequest\"z\n\x16PostEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"i\n\x16ListEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x89\x01\n\x14GetEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\revaluation_id\x18\x02 \x01(\t\x12)\n\x06\x66ields\x18\x03 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"\xb2\x01\n\"PostModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12/\n\x0c\x65val_metrics\x18\x04 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xa1\x01\n\"ListModelVersionEvaluationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xc1\x01\n GetModelVersionEvaluationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x15\n\revaluation_id\x18\x04 \x01(\t\x12)\n\x06\x66ields\x18\x05 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"y\n\x19SingleEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x01(\x0b\x32\x19.clarifai.api.EvalMetrics\"x\n\x18MultiEvalMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\x0c\x65val_metrics\x18\x02 \x03(\x0b\x32\x19.clarifai.api.EvalMetrics\"\xd3\x01\n\x1ePostModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x0btest_search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\x12)\n\teval_info\x18\n \x01(\x0b\x32\x16.clarifai.api.EvalInfoJ\x04\x08\x04\x10\x05\"\xa1\x01\n\x1dGetModelVersionMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x03 \x01(\t\x12)\n\x06\x66ields\x18\x04 \x01(\x0b\x32\x19.clarifai.api.FieldsValue\"]\n\x13GetModelTypeRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x15\n\rmodel_type_id\x18\x02 \x01(\t\"h\n\x15ListModelTypesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x1f\n\x1dListOpenSourceLicensesRequest\"_\n\x1eListOpenSourceLicensesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x10\n\x08licenses\x18\x02 \x03(\t\"y\n\x17SingleModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x31\n\nmodel_type\x18\x02 \x01(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\"\xf2\x01\n\x16MultiModelTypeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bmodel_types\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ModelTypeB\x04\x80\xb5\x18\x01\x12\x35\n\x0fmodel_importers\x18\x03 \x01(\x0b\x32\x1c.clarifai.api.ModelTypeField\x12@\n\x16triton_conda_envs_info\x18\x04 \x03(\x0b\x32 .clarifai.api.TritonCondaEnvInfo\"\x95\x01\n\"GetModelVersionInputExampleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x12\n\nexample_id\x18\x04 \x01(\t\"\xa3\x01\n$ListModelVersionInputExamplesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12\x0c\n\x04page\x18\x04 \x01(\r\x12\x10\n\x08per_page\x18\x05 \x01(\r\"\xa2\x01\n&SingleModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12K\n\x1bmodel_version_input_example\x18\x02 \x01(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\xa2\x01\n%MultiModelVersionInputExampleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cmodel_version_input_examples\x18\x02 \x03(\x0b\x32&.clarifai.api.ModelVersionInputExample\"\x7f\n\x1aListModelReferencesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x82\x01\n\x1bMultiModelReferenceResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10model_references\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.ModelReference\"o\n\x13MultiOutputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07outputs\x18\x02 \x03(\x0b\x32\x14.clarifai.api.OutputB\x04\x80\xb5\x18\x01\"V\n\x11ListScopesRequest\x12\x10\n\x08key_type\x18\x01 \x01(\t\x12/\n\x0buser_app_id\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"B\n\x0fMyScopesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"F\n\x13MyScopesUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x15\n\x13MyScopesRootRequest\"\xa5\x01\n\x16MultiScopeDepsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\nscope_deps\x18\x02 \x03(\x0b\x32\x17.clarifai.api.ScopeDeps\x12\x31\n\rendpoint_deps\x18\x03 \x03(\x0b\x32\x1a.clarifai.api.EndpointDeps\"\xa0\x01\n\x12MultiScopeResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x1e\n\x03\x61pp\x18\x03 \x01(\x0b\x32\x11.clarifai.api.App\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"\x84\x01\n\x16MultiScopeRootResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06scopes\x18\x02 \x03(\t\x12\x11\n\tendpoints\x18\x04 \x03(\t\x12\x1a\n\x12user_feature_flags\x18\x05 \x01(\t\"O\n\x10GetSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"f\n\x13ListSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\xc4\x01\n\x13PostSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x05query\x18\x02 \x01(\x0b\x32\x13.clarifai.api.QueryB\x02\x18\x01\x12&\n\x08searches\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x04 \x01(\x0b\x32\x18.clarifai.api.Pagination\"\x85\x01\n\x1aPatchInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x8a\x01\n\x1fPatchAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x7f\n\x14PatchSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x84\x01\n\x17PostSearchesByIDRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"R\n\x13\x44\x65leteSearchRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xa7\x01\n\x1ePostAnnotationsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\"c\n$DeleteAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\xb6\x01\n\x19PostInputsSearchesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12&\n\x08searches\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Search\x12,\n\npagination\x18\x03 \x01(\x0b\x32\x18.clarifai.api.Pagination\x12\x12\n\nonly_count\x18\x04 \x01(\x08\"i\n\x14SingleSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06search\x18\x05 \x01(\x0b\x32\x14.clarifai.api.Search\"\xed\x01\n\x13MultiSearchResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\n\n\x02id\x18\x02 \x01(\t\x12%\n\x04hits\x18\x03 \x03(\x0b\x32\x11.clarifai.api.HitB\x04\x80\xb5\x18\x01\x12\"\n\x05query\x18\x04 \x01(\x0b\x32\x13.clarifai.api.Query\x12&\n\x08searches\x18\x05 \x03(\x0b\x32\x14.clarifai.api.Search\x12*\n\nhit_counts\x18\x06 \x03(\x0b\x32\x16.clarifai.api.HitCount\"\x94\x02\n\"PostAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\x12*\n\x0cground_truth\x18\x03 \x01(\x0b\x32\x14.clarifai.api.Search\x12,\n\x0esearch_to_eval\x18\x04 \x01(\x0b\x32\x14.clarifai.api.Search\x12 \n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x12.clarifai.api.Data\x12\x35\n\x0f\x65valuation_type\x18\x06 \x01(\x0e\x32\x1c.clarifai.api.EvaluationType\"`\n!GetAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"U\n\"ListAnnotationSearchMetricsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\"\x9d\x01\n$MultiAnnotationSearchMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12H\n\x19\x61nnotation_search_metrics\x18\x02 \x03(\x0b\x32%.clarifai.api.AnnotationSearchMetrics\"o\n\x1cListAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"k\n\x1aGetAnnotationFilterRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1c\n\x14\x61nnotation_filter_id\x18\x02 \x01(\t\"\x8b\x01\n\x1cPostAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\x9c\x01\n\x1dPatchAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12:\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilter\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"p\n\x1e\x44\x65leteAnnotationFiltersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1d\n\x15\x61nnotation_filter_ids\x18\x02 \x03(\t\"\x8e\x01\n\x1dMultiAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x12\x61nnotation_filters\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.AnnotationFilterB\x04\x80\xb5\x18\x01\"\x88\x01\n\x1eSingleAnnotationFilterResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x11\x61nnotation_filter\x18\x02 \x01(\x0b\x32\x1e.clarifai.api.AnnotationFilter\"\\\n\x0eGetUserRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x02 \x03(\t\"c\n\x12SingleUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04user\x18\x02 \x01(\x0b\x32\x12.clarifai.api.User\"x\n\x1bPostValidatePasswordRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12(\n\x08password\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Password\"\x8e\x01\n SinglePasswordValidationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12=\n\x13password_violations\x18\x02 \x01(\x0b\x32 .clarifai.api.PasswordViolations\"\xbb\x01\n\x12GetWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x03 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x04 \x03(\t\x12\"\n\x1a\x65xclude_clarifai_workflows\x18\x05 \x01(\x08\"\x89\x03\n\x14ListWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x16\n\x0esort_ascending\x18\x05 \x01(\x08\x12\x14\n\nsort_by_id\x18\x06 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12sort_by_created_at\x18\r \x01(\x08H\x00\x12\x1c\n\x12sort_by_star_count\x18\x0e \x01(\x08H\x00\x12\r\n\x05query\x18\x08 \x01(\t\x12\x0e\n\x02id\x18\x04 \x01(\tB\x02\x18\x01\x12\x15\n\rfeatured_only\x18\t \x01(\x08\x12\x14\n\x0cstarred_only\x18\x0b \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\n \x03(\t\x12\x13\n\x0bsearch_term\x18\x0c \x01(\t\x12\x10\n\x08\x62ookmark\x18\x0f \x01(\x08\x42\t\n\x07sort_by\"r\n\x14PostWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\"\x83\x01\n\x15PatchWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.Workflow\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"\x85\x01\n\x17PatchWorkflowIdsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12)\n\x03ids\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.IdUpdateSource\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"]\n\x15\x44\x65leteWorkflowRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\"j\n\x16\x44\x65leteWorkflowsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"o\n\x16SingleWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\"u\n\x15MultiWorkflowResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12/\n\tworkflows\x18\x02 \x03(\x0b\x32\x16.clarifai.api.WorkflowB\x04\x80\xb5\x18\x01\"\xa5\x02\n\x1aPostWorkflowResultsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12#\n\x06inputs\x18\x03 \x03(\x0b\x32\x13.clarifai.api.Input\x12\x31\n\routput_config\x18\x04 \x01(\x0b\x32\x1a.clarifai.api.OutputConfig\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x05 \x01(\x08\x12\x33\n\x0eworkflow_state\x18\x06 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\xd8\x01\n\x1bPostWorkflowResultsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12(\n\x08workflow\x18\x02 \x01(\x0b\x32\x16.clarifai.api.Workflow\x12-\n\x07results\x18\x03 \x03(\x0b\x32\x1c.clarifai.api.WorkflowResult\x12\x33\n\x0eworkflow_state\x18\x04 \x01(\x0b\x32\x1b.clarifai.api.WorkflowState\"\x91\x02\n$PostWorkflowResultsSimilarityRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x12\n\nversion_id\x18\x07 \x01(\t\x12\x18\n\x10model_version_id\x18\x03 \x01(\t\x12)\n\x0cprobe_inputs\x18\x04 \x03(\x0b\x32\x13.clarifai.api.Input\x12(\n\x0bpool_inputs\x18\x05 \x03(\x0b\x32\x13.clarifai.api.Input\x12 \n\x18\x66\x61vor_clarifai_workflows\x18\x06 \x01(\x08\"\x8e\x01\n%PostWorkflowResultsSimilarityResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x38\n\x07results\x18\x02 \x03(\x0b\x32\'.clarifai.api.WorkflowResultsSimilarity\"\x83\x01\n\x1bListWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n\x19GetWorkflowVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x03 \x01(\t\"\x83\x01\n\x1d\x44\x65leteWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x1c\n\x14workflow_version_ids\x18\x03 \x03(\t\"\xae\x01\n\x1cPatchWorkflowVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x13\n\x0bworkflow_id\x18\x02 \x01(\t\x12\x38\n\x11workflow_versions\x18\x03 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersion\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\"\x8b\x01\n\x1cMultiWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12>\n\x11workflow_versions\x18\x02 \x03(\x0b\x32\x1d.clarifai.api.WorkflowVersionB\x04\x80\xb5\x18\x01\"\x85\x01\n\x1dSingleWorkflowVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x37\n\x10workflow_version\x18\x02 \x01(\x0b\x32\x1d.clarifai.api.WorkflowVersion\"\x85\x01\n\x1aPostAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"g\n\x18GetAppDuplicationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x1a\n\x12\x61pp_duplication_id\x18\x02 \x01(\t\"m\n\x1aListAppDuplicationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x83\x01\n\x1cMultiAppDuplicationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x36\n\x10\x61pp_duplications\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.AppDuplication\"\x82\x01\n\x1cSingleAppDuplicationResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x35\n\x0f\x61pp_duplication\x18\x02 \x01(\x0b\x32\x1c.clarifai.api.AppDuplication\"f\n\x10PostTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\"m\n\x0eGetTaskRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\xee\x01\n\x10ListTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x17\n\x0fworker_user_ids\x18\x04 \x03(\t\x12\x17\n\x0freview_user_ids\x18\x05 \x03(\t\x12\x17\n\x0flabel_order_ids\x18\x08 \x03(\t\x12#\n\x1bincluding_label_order_tasks\x18\x06 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x07 \x03(\t\"w\n\x11PatchTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12!\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.Task\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"R\n\x12\x44\x65leteTasksRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x11MultiTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\'\n\x05tasks\x18\x02 \x03(\x0b\x32\x12.clarifai.api.TaskB\x04\x80\xb5\x18\x01\"c\n\x12SingleTaskResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12 \n\x04task\x18\x02 \x01(\x0b\x32\x12.clarifai.api.Task\"i\n\x13GetTaskCountRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08user_ids\x18\x03 \x03(\t\"\x9d\x01\n\x17SingleTaskCountResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0f\n\x07task_id\x18\x03 \x01(\t\x12\x34\n\x06\x63ounts\x18\x04 \x03(\x0b\x32$.clarifai.api.TaskStatusCountPerUser\"y\n\x16PostLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\"_\n\x14GetLabelOrderRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x16\n\x0elabel_order_id\x18\x02 \x01(\t\"i\n\x16ListLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x8a\x01\n\x17PatchLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12.\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrder\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"X\n\x18\x44\x65leteLabelOrdersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"|\n\x17MultiLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x34\n\x0clabel_orders\x18\x02 \x03(\x0b\x32\x18.clarifai.api.LabelOrderB\x04\x80\xb5\x18\x01\"v\n\x18SingleLabelOrderResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x0blabel_order\x18\x02 \x01(\x0b\x32\x18.clarifai.api.LabelOrder\"u\n\x15PostCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"\x86\x01\n\x16PatchCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"k\n\x17\x44\x65leteCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\x12\x12\n\ndelete_all\x18\x03 \x01(\x08\"\\\n\x13GetCollectorRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x14\n\x0c\x63ollector_id\x18\x02 \x01(\t\"h\n\x15ListCollectorsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"r\n\x16MultiCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\ncollectors\x18\x02 \x03(\x0b\x32\x17.clarifai.api.Collector\"r\n\x17SingleCollectorResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12*\n\tcollector\x18\x02 \x01(\x0b\x32\x17.clarifai.api.Collector\"v\n\x15PostStatValuesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12,\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValue\"y\n\x16MultiStatValueResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0bstat_values\x18\x02 \x03(\x0b\x32\x17.clarifai.api.StatValueB\x04\x80\xb5\x18\x01\"\x9e\x01\n\x1ePostStatValuesAggregateRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12K\n\x1cstat_value_aggregate_queries\x18\x02 \x03(\x0b\x32%.clarifai.api.StatValueAggregateQuery\"\x9c\x01\n\x1fMultiStatValueAggregateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12L\n\x1cstat_value_aggregate_results\x18\x02 \x03(\x0b\x32&.clarifai.api.StatValueAggregateResult\"w\n\x1ePostTrendingMetricsViewRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x11\n\tobject_id\x18\x03 \x01(\t\"\x85\x01\n\x1fListTrendingMetricsViewsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tview_type\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"~\n MultiTrendingMetricsViewResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x07metrics\x18\x02 \x03(\x0b\x32\x1c.clarifai.api.TrendingMetric\"q\n\x10GetModuleRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x03 \x03(\t\"\xa6\x02\n\x12ListModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\x12\x14\n\x0cstarred_only\x18\x04 \x01(\x08\x12\x19\n\x11\x61\x64\x64itional_fields\x18\x05 \x03(\t\x12\x16\n\x0esort_ascending\x18\x06 \x01(\x08\x12\x1c\n\x12sort_by_created_at\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12sort_by_star_count\x18\x08 \x01(\x08H\x00\x12\x1d\n\x13sort_by_modified_at\x18\t \x01(\x08H\x00\x12\x10\n\x08\x62ookmark\x18\n \x01(\x08\x42\t\n\x07sort_by\"l\n\x12PostModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Module\"}\n\x13PatchModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Module\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\"T\n\x14\x44\x65leteModulesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x14SingleModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06module\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Module\"o\n\x13MultiModuleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07modules\x18\x02 \x03(\x0b\x32\x14.clarifai.api.ModuleB\x04\x80\xb5\x18\x01\"x\n\x17GetModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x19\n\x11module_version_id\x18\x03 \x01(\t\"\x7f\n\x19ListModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0c\n\x04page\x18\x03 \x01(\r\x12\x10\n\x08per_page\x18\x04 \x01(\r\"\x95\x01\n\x19PostModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x34\n\x0fmodule_versions\x18\x03 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersion\"n\n\x1b\x44\x65leteModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tmodule_id\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\t\"\x7f\n\x1bSingleModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0emodule_version\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.ModuleVersion\"\x85\x01\n\x1aMultiModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12:\n\x0fmodule_versions\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.ModuleVersionB\x04\x80\xb5\x18\x01\"x\n GetInstalledModuleVersionRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"u\n\"ListInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x9e\x01\n\"PostInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12G\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersion\"}\n%PostInstalledModuleVersionsKeyRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12#\n\x1binstalled_module_version_id\x18\x02 \x01(\t\"d\n$DeleteInstalledModuleVersionsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x9b\x01\n$SingleInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x46\n\x18installed_module_version\x18\x02 \x01(\x0b\x32$.clarifai.api.InstalledModuleVersion\"\xa1\x01\n#MultiInstalledModuleVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12M\n\x19installed_module_versions\x18\x02 \x03(\x0b\x32$.clarifai.api.InstalledModuleVersionB\x04\x80\xb5\x18\x01\"b\n\x1eListNextTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\x82\x01\n\x19PostBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0f\x62ulk_operations\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"l\n\x19ListBulkOperationsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x17GetBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"Z\n\x1a\x43\x61ncelBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"Z\n\x1a\x44\x65leteBulkOperationRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x80\x01\n\x1cSingleBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x01(\x0b\x32\x1b.clarifai.api.BulkOperation\"\x7f\n\x1bMultiBulkOperationsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x33\n\x0e\x62ulk_operation\x18\x02 \x03(\x0b\x32\x1b.clarifai.api.BulkOperation\"o\n\x19PutTaskAssignmentsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0f\n\x07task_id\x18\x02 \x01(\t\x12\x10\n\x08input_id\x18\x03 \x01(\t\"k\n\x18ListInputsAddJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"U\n\x16GetInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"X\n\x19\x43\x61ncelInputsAddJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\n\n\x02id\x18\x02 \x01(\t\"\x83\x01\n\x19MultiInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x39\n\x0finputs_add_jobs\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsAddJobB\x04\x80\xb5\x18\x01\"}\n\x1aSingleInputsAddJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x32\n\x0einputs_add_job\x18\x02 \x01(\x0b\x32\x1a.clarifai.api.InputsAddJob\"l\n\x12PostUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"T\n\x14\x44\x65leteUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"e\n\x12ListUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"V\n\x10GetUploadRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\"i\n\x14SingleUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06upload\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Upload\"i\n\x13MultiUploadResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12%\n\x07uploads\x18\x02 \x03(\x0b\x32\x14.clarifai.api.Upload\"\x9a\x01\n\x1cPutUploadContentPartsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\tupload_id\x18\x02 \x01(\t\x12\x36\n\rcontent_parts\x18\x03 \x03(\x0b\x32\x1f.clarifai.api.UploadContentPart\"\xad\x01\n\x1cPostInputsDataSourcesRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x34\n\x0c\x64\x61ta_sources\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.InputsDataSource\x12\x15\n\rcall_back_url\x18\x03 \x01(\t\x12\x0f\n\x07\x61pp_pat\x18\x04 \x01(\t\"r\n\x1dGetInputsExtractionJobRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12 \n\x18inputs_extraction_job_id\x18\x02 \x01(\t\"r\n\x1fListInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"\x92\x01\n!SingleInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12@\n\x15inputs_extraction_job\x18\x02 \x01(\x0b\x32!.clarifai.api.InputsExtractionJob\"\x92\x01\n MultiInputsExtractionJobResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x41\n\x16inputs_extraction_jobs\x18\x02 \x03(\x0b\x32!.clarifai.api.InputsExtractionJob\"a\n!CancelInputsExtractionJobsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"\x7f\n\x18PostInputsUploadsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x32\n\x0einputs_uploads\x18\x02 \x03(\x0b\x32\x1a.clarifai.api.InputsUpload\"V\n\x10GetRunnerRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\trunner_id\x18\x02 \x01(\t\"e\n\x12ListRunnersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0c\n\x04page\x18\x02 \x01(\r\x12\x10\n\x08per_page\x18\x03 \x01(\r\"l\n\x12PostRunnersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12%\n\x07runners\x18\x03 \x03(\x0b\x32\x14.clarifai.api.Runner\"T\n\x14\x44\x65leteRunnersRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x0b\n\x03ids\x18\x02 \x03(\t\"i\n\x14SingleRunnerResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12$\n\x06runner\x18\x02 \x01(\x0b\x32\x14.clarifai.api.Runner\"o\n\x13MultiRunnerResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12+\n\x07runners\x18\x02 \x03(\x0b\x32\x14.clarifai.api.RunnerB\x04\x80\xb5\x18\x01\"\\\n\x16ListRunnerItemsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\trunner_id\x18\x02 \x01(\t\"\xb0\x01\n\x1cPostRunnerItemOutputsRequest\x12/\n\x0buser_app_id\x18\x01 \x01(\x0b\x32\x1a.clarifai.api.UserAppIDSet\x12\x11\n\trunner_id\x18\x02 \x01(\t\x12\x0f\n\x07item_id\x18\x03 \x01(\t\x12;\n\x13runner_item_outputs\x18\x04 \x03(\x0b\x32\x1e.clarifai.api.RunnerItemOutput\"u\n\x17MultiRunnerItemResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12-\n\x05items\x18\x02 \x03(\x0b\x32\x18.clarifai.api.RunnerItemB\x04\x80\xb5\x18\x01\"x\n\nRunnerItem\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12I\n\x1apost_model_outputs_request\x18\x03 \x01(\x0b\x32%.clarifai.api.PostModelOutputsRequest\"T\n\x10RunnerItemOutput\x12@\n\x15multi_output_response\x18\x01 \x01(\x0b\x32!.clarifai.api.MultiOutputResponse\"\x8f\x01\n\x1dMultiRunnerItemOutputResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.clarifai.api.status.Status\x12\x41\n\x13runner_item_outputs\x18\x02 \x03(\x0b\x32\x1e.clarifai.api.RunnerItemOutputB\x04\x80\xb5\x18\x01*p\n\x1cOrganizationInvitationStatus\x12\x0b\n\x07NOT_SET\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0c\n\x08\x41\x43\x43\x45PTED\x10\x02\x12\r\n\tCANCELLED\x10\x03\x12\x0c\n\x08\x44\x45\x43LINED\x10\x04\x12\x0b\n\x07\x45XPIRED\x10\x05\x32\x90\x8b\x03\n\x02V2\x12\xae\x02\n\x14ListConceptRelations\x12).clarifai.api.ListConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"\xbe\x01\x82\xd3\xe4\x93\x02\xab\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x0b\x12\xe3\x01\n\x14PostConceptRelations\x12).clarifai.api.PostConceptRelationsRequest\x1a*.clarifai.api.MultiConceptRelationResponse\"t\x82\xd3\xe4\x93\x02^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xe2\x01\n\x16\x44\x65leteConceptRelations\x12+.clarifai.api.DeleteConceptRelationsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\r\x90\x9c\'\n\x90\x9c\'\x0b\x12\xe0\x01\n\x10GetConceptCounts\x12%.clarifai.api.GetConceptCountsRequest\x1a\'.clarifai.api.MultiConceptCountResponse\"|\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/statusZ\x15\x12\x13/v2/concepts/status\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd5\x01\n\nGetConcept\x12\x1f.clarifai.api.GetConceptRequest\x1a#.clarifai.api.SingleConceptResponse\"\x80\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}Z\x1b\x12\x19/v2/concepts/{concept_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xbd\x01\n\x0cListConcepts\x12!.clarifai.api.ListConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/conceptsZ\x0e\x12\x0c/v2/concepts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xbd\x02\n\x11ListModelConcepts\x12&.clarifai.api.ListModelConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"\xdb\x01\x82\xd3\xe4\x93\x02\xc4\x01\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/conceptsZl\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/concepts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xee\x01\n\x14PostConceptsSearches\x12).clarifai.api.PostConceptsSearchesRequest\x1a\".clarifai.api.MultiConceptResponse\"\x86\x01\x82\xd3\xe4\x93\x02l\"K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/searches:\x01*Z\x1a\"\x15/v2/concepts/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xc7\x01\n\x0cPostConcepts\x12!.clarifai.api.PostConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"p\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\"\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xc9\x01\n\rPatchConcepts\x12\".clarifai.api.PatchConceptsRequest\x1a\".clarifai.api.MultiConceptResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts:\x01*Z\x11\x32\x0c/v2/concepts:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x98\x02\n\x12GetConceptLanguage\x12\'.clarifai.api.GetConceptLanguageRequest\x1a+.clarifai.api.SingleConceptLanguageResponse\"\xab\x01\x82\xd3\xe4\x93\x02\x98\x01\x12\x64/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages/{language}Z0\x12./v2/concepts/{concept_id}/languages/{language}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\x85\x02\n\x14ListConceptLanguages\x12).clarifai.api.ListConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x82\x01\x12Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languagesZ%\x12#/v2/concepts/{concept_id}/languages\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\x8f\x02\n\x14PostConceptLanguages\x12).clarifai.api.PostConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9f\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(\"#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x91\x02\n\x15PatchConceptLanguages\x12*.clarifai.api.PatchConceptLanguagesRequest\x1a*.clarifai.api.MultiConceptLanguageResponse\"\x9f\x01\x82\xd3\xe4\x93\x02\x88\x01\x32Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/languages:\x01*Z(2#/v2/concepts/{concept_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\xf5\x01\n\x13ListKnowledgeGraphs\x12(.clarifai.api.ListKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphsZ\x1f\x12\x1d/v2/concepts/knowledge_graphs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x12\xff\x01\n\x13PostKnowledgeGraphs\x12(.clarifai.api.PostKnowledgeGraphsRequest\x1a).clarifai.api.MultiKnowledgeGraphResponse\"\x92\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/knowledge_graphs:\x01*Z\"\"\x1d/v2/concepts/knowledge_graphs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x82\x02\n\x16PostConceptMappingJobs\x12+.clarifai.api.PostConceptMappingJobsRequest\x1a,.clarifai.api.MultiConceptMappingJobResponse\"\x8c\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/mappings/jobs:\x01*Z\x1f\"\x1a/v2/concepts/mappings/jobs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\n\x90\x9c\'\x0b\x12\x97\x02\n\rGetAnnotation\x12\".clarifai.api.GetAnnotationRequest\x1a&.clarifai.api.SingleAnnotationResponse\"\xb9\x01\x82\xd3\xe4\x93\x02\x9e\x01\x12g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3\x12\x31/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xd4\x01\n\x0fListAnnotations\x12$.clarifai.api.ListAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"t\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotationsZ\x11\x12\x0f/v2/annotations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe7\x01\n\x0fPostAnnotations\x12$.clarifai.api.PostAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x86\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\"\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe9\x01\n\x10PatchAnnotations\x12%.clarifai.api.PatchAnnotationsRequest\x1a%.clarifai.api.MultiAnnotationResponse\"\x86\x01\x82\xd3\xe4\x93\x02`2E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14\x32\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf8\x01\n\x16PatchAnnotationsStatus\x12+.clarifai.api.PatchAnnotationsStatusRequest\x1a,.clarifai.api.PatchAnnotationsStatusResponse\"\x82\x01\x82\xd3\xe4\x93\x02`2[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/task/{task_id}/annotations/status:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xa0\x02\n\x10\x44\x65leteAnnotation\x12%.clarifai.api.DeleteAnnotationRequest\x1a!.clarifai.api.status.BaseResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\x9e\x01*g/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/annotations/{annotation_id}Z3*1/v2/inputs/{input_id}/annotations/{annotation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd4\x02\n\x11\x44\x65leteAnnotations\x12&.clarifai.api.DeleteAnnotationsRequest\x1a!.clarifai.api.status.BaseResponse\"\xf3\x01\x82\xd3\xe4\x93\x02\xd0\x01*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/annotations:\x01*Z\x1b*\x16/v2/inputs/annotations:\x01*ZJ*E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations:\x01*Z\x14*\x0f/v2/annotations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf7\x01\n\x18PatchAnnotationsSearches\x12-.clarifai.api.PatchAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x88\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\x32\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\x85\x02\n\x17PostAnnotationsSearches\x12,.clarifai.api.PostAnnotationsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x98\x01\x82\xd3\xe4\x93\x02r\"N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches:\x01*Z\x1d\"\x18/v2/annotations/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd5\x01\n\rGetInputCount\x12\".clarifai.api.GetInputCountRequest\x1a&.clarifai.api.SingleInputCountResponse\"x\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/statusZ\x13\x12\x11/v2/inputs/status\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xcd\x01\n\x0cStreamInputs\x12!.clarifai.api.StreamInputsRequest\x1a .clarifai.api.MultiInputResponse\"x\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/streamZ\x13\x12\x11/v2/inputs/stream\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x81\x02\n\x0fGetInputSamples\x12$.clarifai.api.GetInputSamplesRequest\x1a*.clarifai.api.MultiInputAnnotationResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/samplesZ$\x12\"/v2/tasks/{task_id}/inputs/samples\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xcf\x01\n\x08GetInput\x12\x1d.clarifai.api.GetInputRequest\x1a!.clarifai.api.SingleInputResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17\x12\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x80\x02\n\x15GetInputVideoManifest\x12%.clarifai.api.GetVideoManifestRequest\x1a&.clarifai.api.GetVideoManifestResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}/video_manifestZ&\x12$/v2/inputs/{input_id}/video_manifest\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xbb\x01\n\nListInputs\x12\x1f.clarifai.api.ListInputsRequest\x1a .clarifai.api.MultiInputResponse\"j\x82\xd3\xe4\x93\x02P\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputsZ\x0c\x12\n/v2/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\xd6\x01\n\nPostInputs\x12\x1f.clarifai.api.PostInputsRequest\x1a .clarifai.api.MultiInputResponse\"\x84\x01\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\"\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xcf\x01\n\x0bPatchInputs\x12 .clarifai.api.PatchInputsRequest\x1a .clarifai.api.MultiInputResponse\"|\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f\x32\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x12\xe9\x01\n\x0b\x44\x65leteInput\x12 .clarifai.api.DeleteInputRequest\x1a!.clarifai.api.status.BaseResponse\"\x94\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/{input_id}Z\x17*\x15/v2/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xdb\x01\n\x0c\x44\x65leteInputs\x12!.clarifai.api.DeleteInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs:\x01*Z\x0f*\n/v2/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'(\x90\x9c\'&\x90\x9c\'\x04\x90\x9c\'\x08\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xe2\x01\n\x13PatchInputsSearches\x12(.clarifai.api.PatchInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"~\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\x32\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\xf1\x01\n\x12PostInputsSearches\x12\'.clarifai.api.PostInputsSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x8e\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/searches:\x01*Z\x18\"\x13/v2/inputs/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xa0\x03\n\x10PostModelOutputs\x12%.clarifai.api.PostModelOutputsRequest\x1a!.clarifai.api.MultiOutputResponse\"\xc1\x02\x82\xd3\xe4\x93\x02\xa6\x02\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/outputs:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/outputs:\x01*ZX\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/outputs:\x01*Z\"\"\x1d/v2/models/{model_id}/outputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x02\x12\xef\x01\n\x0cListDatasets\x12!.clarifai.api.ListDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasetsZ*\x12(/v2/users/{user_app_id.user_id}/datasetsZ\x0e\x12\x0c/v2/datasets\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xd9\x01\n\nGetDataset\x12\x1f.clarifai.api.GetDatasetRequest\x1a#.clarifai.api.SingleDatasetResponse\"\x84\x01\x82\xd3\xe4\x93\x02n\x12O/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}Z\x1b\x12\x19/v2/datasets/{dataset_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xcb\x01\n\x0cPostDatasets\x12!.clarifai.api.PostDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"t\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\"\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xcd\x01\n\rPatchDatasets\x12\".clarifai.api.PatchDatasetsRequest\x1a\".clarifai.api.MultiDatasetResponse\"t\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11\x32\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'r\x12\xce\x01\n\x0e\x44\x65leteDatasets\x12#.clarifai.api.DeleteDatasetsRequest\x1a!.clarifai.api.status.BaseResponse\"t\x82\xd3\xe4\x93\x02Z*B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets:\x01*Z\x11*\x0c/v2/datasets:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\x81\x02\n\x11ListDatasetInputs\x12&.clarifai.api.ListDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\x9a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputsZ\"\x12 /v2/datasets/{dataset_id}/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x95\x02\n\x0fGetDatasetInput\x12$.clarifai.api.GetDatasetInputRequest\x1a(.clarifai.api.SingleDatasetInputResponse\"\xb1\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs/{input_id}Z-\x12+/v2/datasets/{dataset_id}/inputs/{input_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x8c\x02\n\x11PostDatasetInputs\x12&.clarifai.api.PostDatasetInputsRequest\x1a\'.clarifai.api.MultiDatasetInputResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%\" /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x05\x90\x9c\'&\x90\x9c\'\x0b\x12\x86\x02\n\x13\x44\x65leteDatasetInputs\x12(.clarifai.api.DeleteDatasetInputsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x82\x01*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/inputs:\x01*Z%* /v2/datasets/{dataset_id}/inputs:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x90\x9c\'\x05\x12\x84\x02\n\x13ListDatasetVersions\x12(.clarifai.api.ListDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x97\x01\x82\xd3\xe4\x93\x02\x80\x01\x12X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versionsZ$\x12\"/v2/datasets/{dataset_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xab\x02\n\x11GetDatasetVersion\x12&.clarifai.api.GetDatasetVersionRequest\x1a*.clarifai.api.SingleDatasetVersionResponse\"\xc1\x01\x82\xd3\xe4\x93\x02\xaa\x01\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}Z9\x12\x37/v2/datasets/{dataset_id}/versions/{dataset_version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'r\x12\xea\x02\n\x1fListDatasetVersionMetricsGroups\x12\x34.clarifai.api.ListDatasetVersionMetricsGroupsRequest\x1a\x35.clarifai.api.MultiDatasetVersionMetricsGroupResponse\"\xd9\x01\x82\xd3\xe4\x93\x02\xba\x01\x12u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/metricsZA\x12?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x12\x92\x02\n\x13PostDatasetVersions\x12(.clarifai.api.PostDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x86\x01\"X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'\"\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x8c\x02\n\x14PatchDatasetVersions\x12).clarifai.api.PatchDatasetVersionsRequest\x1a).clarifai.api.MultiDatasetVersionResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x86\x01\x32X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'2\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x12\x8a\x02\n\x15\x44\x65leteDatasetVersions\x12*.clarifai.api.DeleteDatasetVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01*X/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions:\x01*Z\'*\"/v2/datasets/{dataset_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x90\x9c\'k\x12\xd4\x02\n\x18PutDatasetVersionExports\x12-.clarifai.api.PutDatasetVersionExportsRequest\x1a/.clarifai.api.MultiDatasetVersionExportResponse\"\xd7\x01\x82\xd3\xe4\x93\x02\xc0\x01\x1au/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*ZD\x1a?/v2/datasets/{dataset_id}/versions/{dataset_version_id}/exports:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x90\x9c\'j\x12\xe9\x01\n\x0cGetModelType\x12!.clarifai.api.GetModelTypeRequest\x1a%.clarifai.api.SingleModelTypeResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/types/{model_type_id}Z\"\x12 /v2/models/types/{model_type_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\x99\x01\n\x16ListOpenSourceLicenses\x12+.clarifai.api.ListOpenSourceLicensesRequest\x1a,.clarifai.api.ListOpenSourceLicensesResponse\"$\x82\xd3\xe4\x93\x02\x1a\x12\x18/v2/open_source_licenses\x98\x9c\'\x01\x12\xcb\x01\n\x0eListModelTypes\x12#.clarifai.api.ListModelTypesRequest\x1a$.clarifai.api.MultiModelTypeResponse\"n\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/typesZ\x12\x12\x10/v2/models/types\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xca\x01\n\x08GetModel\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"|\x82\xd3\xe4\x93\x02\x66\x12K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17\x12\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\x9a\x03\n\x12GetModelOutputInfo\x12\x1d.clarifai.api.GetModelRequest\x1a!.clarifai.api.SingleModelResponse\"\xc1\x02\x82\xd3\xe4\x93\x02\xaa\x02\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/output_infoZ#\x12!/v2/models/{model_id}/output_infoZo\x12m/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/output_infoZ9\x12\x37/v2/models/{model_id}/versions/{version_id}/output_info\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe2\x01\n\nListModels\x12\x1f.clarifai.api.ListModelsRequest\x1a .clarifai.api.MultiModelResponse\"\x90\x01\x82\xd3\xe4\x93\x02z\x12@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modelsZ(\x12&/v2/users/{user_app_id.user_id}/modelsZ\x0c\x12\n/v2/models\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xe7\x01\n\x11GetResourceCounts\x12&.clarifai.api.GetResourceCountsRequest\x1a\'.clarifai.api.GetResourceCountsResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/resource_countsZ\x15\x12\x13/v2/resource_counts\x98\x9c\'\x02\x90\x9c\'i\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'m\x90\x9c\'-\x12\xdf\x01\n\x12PostModelsSearches\x12\'.clarifai.api.PostModelsSearchesRequest\x1a .clarifai.api.MultiModelResponse\"~\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/searches:\x01*Z\x18\"\x13/v2/models/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xca\x01\n\nPostModels\x12\x1f.clarifai.api.PostModelsRequest\x1a!.clarifai.api.SingleModelResponse\"x\x82\xd3\xe4\x93\x02V\"@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\"\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x12\xc7\x01\n\x0bPatchModels\x12 .clarifai.api.PatchModelsRequest\x1a .clarifai.api.MultiModelResponse\"t\x82\xd3\xe4\x93\x02V2@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f\x32\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x12\xb6\x01\n\rPatchModelIds\x12\".clarifai.api.PatchModelIdsRequest\x1a .clarifai.api.MultiModelResponse\"_\x82\xd3\xe4\x93\x02I2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/ids:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0e\x90\x9c\'\x0f\x12\xdd\x01\n\x0b\x44\x65leteModel\x12 .clarifai.api.DeleteModelRequest\x1a!.clarifai.api.status.BaseResponse\"\x88\x01\x82\xd3\xe4\x93\x02\x66*K/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}Z\x17*\x15/v2/models/{model_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xce\x01\n\x0c\x44\x65leteModels\x12!.clarifai.api.DeleteModelsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02V*@/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models:\x01*Z\x0f*\n/v2/models:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x95\x02\n\x17PatchModelCheckConsents\x12,.clarifai.api.PatchModelCheckConsentsRequest\x1a,.clarifai.api.MultiModelCheckConsentResponse\"\x9d\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/check_consents:\x01*Z)2$/v2/models/{model_id}/check_consents:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf9\x01\n\x12PatchModelToolkits\x12\'.clarifai.api.PatchModelToolkitsRequest\x1a\'.clarifai.api.MultiModelToolkitResponse\"\x90\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/toolkits:\x01*Z#2\x1e/v2/models/{model_id}/toolkits:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf9\x01\n\x12PatchModelUseCases\x12\'.clarifai.api.PatchModelUseCasesRequest\x1a\'.clarifai.api.MultiModelUseCaseResponse\"\x90\x01\x82\xd3\xe4\x93\x02~2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/usecases:\x01*Z#2\x1e/v2/models/{model_id}/usecases:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xff\x01\n\x13PatchModelLanguages\x12(.clarifai.api.PatchModelLanguagesRequest\x1a(.clarifai.api.MultiModelLanguageResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x80\x01\x32U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/languages:\x01*Z$2\x1f/v2/models/{model_id}/languages:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\x91\x03\n\x0fListModelInputs\x12$.clarifai.api.ListModelInputsRequest\x1a .clarifai.api.MultiInputResponse\"\xb5\x02\x82\xd3\xe4\x93\x02\x96\x02\x12R/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/inputsZ\x1e\x12\x1c/v2/models/{model_id}/inputsZj\x12h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/inputsZ4\x12\x32/v2/models/{model_id}/versions/{version_id}/inputs\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x12\x8d\x02\n\x0fGetModelVersion\x12$.clarifai.api.GetModelVersionRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x92\x01\x12\x61/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-\x12+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xf5\x01\n\x11ListModelVersions\x12&.clarifai.api.ListModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"\x8e\x01\x82\xd3\xe4\x93\x02x\x12T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versionsZ \x12\x1e/v2/models/{model_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x12\xbc\x02\n\x1dPostWorkflowVersionsUnPublish\x12\x32.clarifai.api.PostWorkflowVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xc3\x01\x82\xd3\xe4\x93\x02\x8c\x01\"[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/unpublish:\x01*Z*\"%/v2/workflows/{workflow_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'x\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xb4\x02\n\x1bPostWorkflowVersionsPublish\x12\x30.clarifai.api.PostWorkflowVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xbf\x01\x82\xd3\xe4\x93\x02\x88\x01\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/publish:\x01*Z(\"#/v2/workflows/{workflow_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'w\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xa1\x02\n\x18PostModelVersionsPublish\x12-.clarifai.api.PostModelVersionsPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb2\x01\x82\xd3\xe4\x93\x02|\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/publish:\x01*Z\"\"\x1d/v2/models/{model_id}/publish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'u\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xaa\x02\n\x1aPostModelVersionsUnPublish\x12/.clarifai.api.PostModelVersionsUnPublishRequest\x1a!.clarifai.api.status.BaseResponse\"\xb7\x01\x82\xd3\xe4\x93\x02\x80\x01\"U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/unpublish:\x01*Z$\"\x1f/v2/models/{model_id}/unpublish:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'v\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\x91\x02\n\x11PostModelVersions\x12&.clarifai.api.PostModelVersionsRequest\x1a!.clarifai.api.SingleModelResponse\"\xb0\x01\x82\xd3\xe4\x93\x02~\"T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*Z#\"\x1e/v2/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdf\x01\n\x12PatchModelVersions\x12\'.clarifai.api.PatchModelVersionsRequest\x1a\'.clarifai.api.MultiModelVersionResponse\"w\x82\xd3\xe4\x93\x02Y2T/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x0e\x90\x9c\'\x1a\x12\x98\x02\n\x12\x44\x65leteModelVersion\x12\'.clarifai.api.DeleteModelVersionRequest\x1a!.clarifai.api.status.BaseResponse\"\xb5\x01\x82\xd3\xe4\x93\x02\x92\x01*a/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}Z-*+/v2/models/{model_id}/versions/{version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0b\x90\x9c\'\x0e\x90\x9c\'\x11\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb7\x02\n\x16GetModelVersionMetrics\x12+.clarifai.api.GetModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xc5\x01\x82\xd3\xe4\x93\x02\xa2\x01\x12i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metricsZ5\x12\x33/v2/models/{model_id}/versions/{version_id}/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xd3\x02\n\x17PostModelVersionMetrics\x12,.clarifai.api.PostModelVersionMetricsRequest\x1a(.clarifai.api.SingleModelVersionResponse\"\xdf\x01\x82\xd3\xe4\x93\x02\xa8\x01\"i/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{version_id}/metrics:\x01*Z8\"3/v2/models/{model_id}/versions/{version_id}/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xed\x02\n\x1bPostModelVersionEvaluations\x12\x30.clarifai.api.PostModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xf3\x01\x82\xd3\xe4\x93\x02\xbc\x01\"s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations:\x01*ZB\"=/v2/models/{model_id}/versions/{model_version_id}/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xd3\x02\n\x1bListModelVersionEvaluations\x12\x30.clarifai.api.ListModelVersionEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\xd9\x01\x82\xd3\xe4\x93\x02\xb6\x01\x12s/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluationsZ?\x12=/v2/models/{model_id}/versions/{model_version_id}/evaluations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf1\x02\n\x19GetModelVersionEvaluation\x12..clarifai.api.GetModelVersionEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\xfa\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xf8\x01\n\x0fPostEvaluations\x12$.clarifai.api.PostEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"\x96\x01\x82\xd3\xe4\x93\x02`\"E/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations:\x01*Z\x14\"\x0f/v2/evaluations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'5\x90\x9c\'6\x12\xdd\x01\n\x0fListEvaluations\x12$.clarifai.api.ListEvaluationsRequest\x1a&.clarifai.api.MultiEvalMetricsResponse\"|\x82\xd3\xe4\x93\x02Z\x12\x45/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluationsZ\x11\x12\x0f/v2/evaluations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xfb\x01\n\rGetEvaluation\x12\".clarifai.api.GetEvaluationRequest\x1a\'.clarifai.api.SingleEvalMetricsResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/evaluations/{evaluation_id}Z!\x12\x1f/v2/evaluations/{evaluation_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x0f\x90\x9c\'\x05\x90\x9c\'5\x12\xfb\x01\n\x13ListModelReferences\x12(.clarifai.api.ListModelReferencesRequest\x1a).clarifai.api.MultiModelReferenceResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/referencesZ\"\x12 /v2/models/{model_id}/references\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xf2\x02\n\x1bGetModelVersionInputExample\x12\x30.clarifai.api.GetModelVersionInputExampleRequest\x1a\x34.clarifai.api.SingleModelVersionInputExampleResponse\"\xea\x01\x82\xd3\xe4\x93\x02\xd7\x01\x12\x83\x01/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}ZO\x12M/v2/models/{model_id}/versions/{model_version_id}/input_examples/{example_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xda\x02\n\x1dListModelVersionInputExamples\x12\x32.clarifai.api.ListModelVersionInputExamplesRequest\x1a\x33.clarifai.api.MultiModelVersionInputExampleResponse\"\xcf\x01\x82\xd3\xe4\x93\x02\xbc\x01\x12v/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/models/{model_id}/versions/{model_version_id}/input_examplesZB\x12@/v2/models/{model_id}/versions/{model_version_id}/input_examples\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x12\xe0\x01\n\x0bGetWorkflow\x12 .clarifai.api.GetWorkflowRequest\x1a$.clarifai.api.SingleWorkflowResponse\"\x88\x01\x82\xd3\xe4\x93\x02r\x12Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d\x12\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xf5\x01\n\rListWorkflows\x12\".clarifai.api.ListWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"\x9a\x01\x82\xd3\xe4\x93\x02\x83\x01\x12\x43/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflowsZ+\x12)/v2/users/{user_app_id.user_id}/workflowsZ\x0f\x12\r/v2/workflows\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xd0\x01\n\rPostWorkflows\x12\".clarifai.api.PostWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"v\x82\xd3\xe4\x93\x02\\\"C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\"\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xd2\x01\n\x0ePatchWorkflows\x12#.clarifai.api.PatchWorkflowsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"v\x82\xd3\xe4\x93\x02\\2C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12\x32\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x12\x90\x9c\'\x13\x12\xc2\x01\n\x10PatchWorkflowIds\x12%.clarifai.api.PatchWorkflowIdsRequest\x1a#.clarifai.api.MultiWorkflowResponse\"b\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/ids:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x13\x12\xe7\x01\n\x0e\x44\x65leteWorkflow\x12#.clarifai.api.DeleteWorkflowRequest\x1a!.clarifai.api.status.BaseResponse\"\x8c\x01\x82\xd3\xe4\x93\x02r*Q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}Z\x1d*\x1b/v2/workflows/{workflow_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\xd2\x01\n\x0f\x44\x65leteWorkflows\x12$.clarifai.api.DeleteWorkflowsRequest\x1a!.clarifai.api.status.BaseResponse\"v\x82\xd3\xe4\x93\x02\\*C/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows:\x01*Z\x12*\r/v2/workflows:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x12\x90\x9c\'\x15\x90\x9c\'\x13\x12\x8a\x03\n\x13PostWorkflowResults\x12(.clarifai.api.PostWorkflowResultsRequest\x1a).clarifai.api.PostWorkflowResultsResponse\"\x9d\x02\x82\xd3\xe4\x93\x02\xfe\x01\"o/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results:\x01*Z^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results:\x01*Z(\"#/v2/workflows/{workflow_id}/results:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\xc9\x03\n\x1dPostWorkflowResultsSimilarity\x12\x32.clarifai.api.PostWorkflowResultsSimilarityRequest\x1a\x33.clarifai.api.PostWorkflowResultsSimilarityResponse\"\xbe\x02\x82\xd3\xe4\x93\x02\x9f\x02\"z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{version_id}/results/similarity:\x01*Zi\"d/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/results/similarity:\x01*Z3\"./v2/workflows/{workflow_id}/results/similarity:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x0b\x90\x9c\'\x02\x90\x9c\'\x13\x12\x8b\x02\n\x14ListWorkflowVersions\x12).clarifai.api.ListWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\x9b\x01\x82\xd3\xe4\x93\x02\x84\x01\x12Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versionsZ&\x12$/v2/workflows/{workflow_id}/versions\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xb4\x02\n\x12GetWorkflowVersion\x12\'.clarifai.api.GetWorkflowVersionRequest\x1a+.clarifai.api.SingleWorkflowVersionResponse\"\xc7\x01\x82\xd3\xe4\x93\x02\xb0\x01\x12p/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions/{workflow_version_id}Z<\x12:/v2/workflows/{workflow_id}/versions/{workflow_version_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x12\x90\x02\n\x16\x44\x65leteWorkflowVersions\x12+.clarifai.api.DeleteWorkflowVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x8a\x01*Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)*$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x13\x90\x9c\'\x12\x90\x9c\'\x15\x12\x97\x02\n\x15PatchWorkflowVersions\x12*.clarifai.api.PatchWorkflowVersionsRequest\x1a*.clarifai.api.MultiWorkflowVersionResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x8a\x01\x32Z/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/workflows/{workflow_id}/versions:\x01*Z)2$/v2/workflows/{workflow_id}/versions:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x85\x01\n\x06GetKey\x12\x1b.clarifai.api.GetKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"=\x82\xd3\xe4\x93\x02/\x12-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'0\x12\x7f\n\x08ListKeys\x12\x1d.clarifai.api.ListKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"4\x82\xd3\xe4\x93\x02&\x12$/v2/users/{user_app_id.user_id}/keys\x98\x9c\'\x05\x90\x9c\'0\x12\xa3\x01\n\x0bListAppKeys\x12 .clarifai.api.ListAppKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"R\x82\xd3\xe4\x93\x02@\x12>/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/keys\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'0\x12\x95\x01\n\tDeleteKey\x12\x1e.clarifai.api.DeleteKeyRequest\x1a!.clarifai.api.status.BaseResponse\"E\x82\xd3\xe4\x93\x02/*-/v2/users/{user_app_id.user_id}/keys/{key_id}\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'1\x90\x9c\'0\x12\x8a\x01\n\x08PostKeys\x12\x1d.clarifai.api.PostKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\"?\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\x88\x01\n\tPatchKeys\x12\x1e.clarifai.api.PatchKeysRequest\x1a\x1e.clarifai.api.MultiKeyResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/keys:\x01*\x98\x9c\'\x05\x90\x9c\'/\x90\x9c\'0\x12\xbc\x01\n\x08MyScopes\x12\x1d.clarifai.api.MyScopesRequest\x1a .clarifai.api.MultiScopeResponse\"o\x82\xd3\xe4\x93\x02\x65\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/myscopesZ\x0e\x12\x0c/v2/myscopesZ\x0f\x12\r/v2/my_scopes\x98\x9c\'\x02\x12\x8d\x01\n\x0cMyScopesUser\x12!.clarifai.api.MyScopesUserRequest\x1a$.clarifai.api.MultiScopeUserResponse\"4\x82\xd3\xe4\x93\x02*\x12(/v2/users/{user_app_id.user_id}/myscopes\x98\x9c\'\x05\x12u\n\x0cMyScopesRoot\x12!.clarifai.api.MyScopesRootRequest\x1a$.clarifai.api.MultiScopeRootResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/myscopesroot\x98\x9c\'\x05\x12\x87\x01\n\nListScopes\x12\x1f.clarifai.api.ListScopesRequest\x1a$.clarifai.api.MultiScopeDepsResponse\"2\x82\xd3\xe4\x93\x02(\x12&/v2/users/{user_app_id.user_id}/scopes\x98\x9c\'\x03\x12\x95\x01\n\x06GetApp\x12\x1b.clarifai.api.GetAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"M\x82\xd3\xe4\x93\x02;\x12\x39/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\x8f\x01\n\x08ListApps\x12\x1d.clarifai.api.ListAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\x12$/v2/users/{user_app_id.user_id}/appsZ\n\x12\x08/v2/apps\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12\xa5\x01\n\tDeleteApp\x12\x1e.clarifai.api.DeleteAppRequest\x1a!.clarifai.api.status.BaseResponse\"U\x82\xd3\xe4\x93\x02;*9/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'.\x90\x9c\'-\x90\x9c\'\x13\x12\x92\x01\n\x08PostApps\x12\x1d.clarifai.api.PostAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"G\x82\xd3\xe4\x93\x02)\"$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x90\x9c\'\x0f\x90\x9c\'\x13\x90\x9c\'\x12\x12\x88\x01\n\tPatchApps\x12\x1e.clarifai.api.PatchAppsRequest\x1a\x1e.clarifai.api.MultiAppResponse\";\x82\xd3\xe4\x93\x02)2$/v2/users/{user_app_id.user_id}/apps:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x92\x01\n\x0cPatchAppsIds\x12!.clarifai.api.PatchAppsIdsRequest\x1a\x1e.clarifai.api.MultiAppResponse\"?\x82\xd3\xe4\x93\x02-2(/v2/users/{user_app_id.user_id}/apps/ids:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9c\x01\n\x08PatchApp\x12\x1d.clarifai.api.PatchAppRequest\x1a\x1f.clarifai.api.SingleAppResponse\"P\x82\xd3\xe4\x93\x02>29/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}:\x01*\x98\x9c\'\x05\x90\x9c\',\x90\x9c\'-\x12\x9f\x01\n\x10PostAppsSearches\x12%.clarifai.api.PostAppsSearchesRequest\x1a\x1e.clarifai.api.MultiAppResponse\"D\x82\xd3\xe4\x93\x02\x32\"-/v2/users/{user_app_id.user_id}/apps/searches:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x13\x12v\n\x07GetUser\x12\x1c.clarifai.api.GetUserRequest\x1a .clarifai.api.SingleUserResponse\"+\x82\xd3\xe4\x93\x02!\x12\x1f/v2/users/{user_app_id.user_id}\x98\x9c\'\x05\x12\xcf\x01\n\x14PostValidatePassword\x12).clarifai.api.PostValidatePasswordRequest\x1a..clarifai.api.SinglePasswordValidationResponse\"\\\x82\xd3\xe4\x93\x02R\"1/v2/users/{user_app_id.user_id}/validate_password:\x01*Z\x1a\"\x15/v2/validate_password:\x01*\x98\x9c\'\x03\x12\xc1\x01\n\tGetSearch\x12\x1e.clarifai.api.GetSearchRequest\x1a\".clarifai.api.SingleSearchResponse\"p\x82\xd3\xe4\x93\x02^\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13\x12\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xbc\x01\n\x0cListSearches\x12!.clarifai.api.ListSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"f\x82\xd3\xe4\x93\x02T\x12\x42/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searchesZ\x0e\x12\x0c/v2/searches\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xc8\x01\n\rPatchSearches\x12\".clarifai.api.PatchSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"p\x82\xd3\xe4\x93\x02Z2B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\x32\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'s\x90\x9c\'r\x12\xda\x01\n\x0cPostSearches\x12!.clarifai.api.PostSearchesRequest\x1a!.clarifai.api.MultiSearchResponse\"\x83\x01\x88\x02\x01\x82\xd3\xe4\x93\x02Z\"B/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches:\x01*Z\x11\"\x0c/v2/searches:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x03\x90\x9c\'\x13\x12\xd8\x01\n\x10PostSearchesByID\x12%.clarifai.api.PostSearchesByIDRequest\x1a!.clarifai.api.MultiSearchResponse\"z\x82\xd3\xe4\x93\x02\x64\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}:\x01*Z\x16\"\x11/v2/searches/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'\x03\x12\xb3\x02\n\x1bPostAnnotationSearchMetrics\x12\x30.clarifai.api.PostAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xad\x01\x82\xd3\xe4\x93\x02\x82\x01\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics:\x01*Z%\" /v2/annotations/searches/metrics:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x90\x9c\'6\x90\x9c\'\x0f\x90\x9c\'\x13\x12\xa9\x02\n\x1aGetAnnotationSearchMetrics\x12/.clarifai.api.GetAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\xa5\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'\x12%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\xa0\x02\n\x1bListAnnotationSearchMetrics\x12\x30.clarifai.api.ListAnnotationSearchMetricsRequest\x1a\x32.clarifai.api.MultiAnnotationSearchMetricsResponse\"\x9a\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metricsZ\"\x12 /v2/annotations/searches/metrics\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'5\x12\x9a\x02\n\x1d\x44\x65leteAnnotationSearchMetrics\x12\x32.clarifai.api.DeleteAnnotationSearchMetricsRequest\x1a!.clarifai.api.status.BaseResponse\"\xa1\x01\x82\xd3\xe4\x93\x02\x86\x01*[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotations/searches/metrics/{id}Z\'*%/v2/annotations/searches/metrics/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'5\x90\x9c\'6\x90\x9c\'?\x12\xce\x01\n\x0c\x44\x65leteSearch\x12!.clarifai.api.DeleteSearchRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/searches/{id}Z\x13*\x11/v2/searches/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x90\x9c\'t\x12\xec\x01\n\x15ListAnnotationFilters\x12*.clarifai.api.ListAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"z\x82\xd3\xe4\x93\x02h\x12L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filtersZ\x18\x12\x16/v2/annotation_filters\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\x99\x02\n\x13GetAnnotationFilter\x12(.clarifai.api.GetAnnotationFilterRequest\x1a,.clarifai.api.SingleAnnotationFilterResponse\"\xa9\x01\x82\xd3\xe4\x93\x02\x96\x01\x12\x63/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters/{annotation_filter_id}Z/\x12-/v2/annotation_filters/{annotation_filter_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x12\xf7\x01\n\x15PostAnnotationFilters\x12*.clarifai.api.PostAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x84\x01\x82\xd3\xe4\x93\x02n\"L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\"\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12\xf9\x01\n\x16PatchAnnotationFilters\x12+.clarifai.api.PatchAnnotationFiltersRequest\x1a+.clarifai.api.MultiAnnotationFilterResponse\"\x84\x01\x82\xd3\xe4\x93\x02n2L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b\x32\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12\xf1\x01\n\x17\x44\x65leteAnnotationFilters\x12,.clarifai.api.DeleteAnnotationFiltersRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02n*L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/annotation_filters:\x01*Z\x1b*\x16/v2/annotation_filters:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'r\x90\x9c\'s\x12|\n\x0fListStatusCodes\x12$.clarifai.api.ListStatusCodesRequest\x1a%.clarifai.api.MultiStatusCodeResponse\"\x1c\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/status_codes\x98\x9c\'\x01\x12\x8a\x01\n\rGetStatusCode\x12\".clarifai.api.GetStatusCodeRequest\x1a&.clarifai.api.SingleStatusCodeResponse\"-\x82\xd3\xe4\x93\x02#\x12!/v2/status_codes/{status_code_id}\x98\x9c\'\x01\x12\xc2\x01\n\x11ListCollaborators\x12&.clarifai.api.ListCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"[\x82\xd3\xe4\x93\x02I\x12G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'2\x12\xc9\x01\n\x11PostCollaborators\x12&.clarifai.api.PostCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"b\x82\xd3\xe4\x93\x02L\"G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x12\xcf\x01\n\x12PatchCollaborators\x12\'.clarifai.api.PatchCollaboratorsRequest\x1a(.clarifai.api.MultiCollaboratorsResponse\"f\x82\xd3\xe4\x93\x02L2G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x12\xd2\x01\n\x13\x44\x65leteCollaborators\x12(.clarifai.api.DeleteCollaboratorsRequest\x1a!.clarifai.api.status.BaseResponse\"n\x82\xd3\xe4\x93\x02L*G/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collaborators:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'3\x90\x9c\'2\x90\x9c\'4\x90\x9c\'7\x90\x9c\'8\x12\xa4\x01\n\x12ListCollaborations\x12\'.clarifai.api.ListCollaborationsRequest\x1a).clarifai.api.MultiCollaborationsResponse\":\x82\xd3\xe4\x93\x02\x30\x12./v2/users/{user_app_id.user_id}/collaborations\x98\x9c\'\x03\x12\xf3\x01\n\x13PostAppDuplications\x12(.clarifai.api.PostAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"\x85\x01\x82\xd3\xe4\x93\x02K\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/duplications:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x0e\x90\x9c\'\x0f\x90\x9c\'\x1a\x90\x9c\'\n\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x12\x90\x9c\'\x13\x12\xa5\x01\n\x13ListAppDuplications\x12(.clarifai.api.ListAppDuplicationsRequest\x1a*.clarifai.api.MultiAppDuplicationsResponse\"8\x82\xd3\xe4\x93\x02.\x12,/v2/users/{user_app_id.user_id}/duplications\x98\x9c\'\x05\x12\xb6\x01\n\x11GetAppDuplication\x12&.clarifai.api.GetAppDuplicationRequest\x1a*.clarifai.api.SingleAppDuplicationResponse\"M\x82\xd3\xe4\x93\x02\x43\x12\x41/v2/users/{user_app_id.user_id}/duplications/{app_duplication_id}\x98\x9c\'\x05\x12\xd9\x01\n\tPostTasks\x12\x1e.clarifai.api.PostTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x8a\x01\x82\xd3\xe4\x93\x02T\"?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\"\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'\x03\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xfe\x01\n\x16GetTaskAnnotationCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x99\x01\x82\xd3\xe4\x93\x02\x86\x01\x12[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/annotations/countZ\'\x12%/v2/tasks/{task_id}/annotations/count\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x12\xee\x01\n\x11GetTaskInputCount\x12!.clarifai.api.GetTaskCountRequest\x1a%.clarifai.api.SingleTaskCountResponse\"\x8e\x01\x82\xd3\xe4\x93\x02|\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/inputs/countZ\"\x12 /v2/tasks/{task_id}/inputs/count\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x12\xd0\x01\n\x07GetTask\x12\x1c.clarifai.api.GetTaskRequest\x1a .clarifai.api.SingleTaskResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}Z\x15\x12\x13/v2/tasks/{task_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xbe\x01\n\tListTasks\x12\x1e.clarifai.api.ListTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"p\x82\xd3\xe4\x93\x02N\x12?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasksZ\x0b\x12\t/v2/tasks\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'8\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xd7\x01\n\nPatchTasks\x12\x1f.clarifai.api.PatchTasksRequest\x1a\x1f.clarifai.api.MultiTaskResponse\"\x86\x01\x82\xd3\xe4\x93\x02T2?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e\x32\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x90\x9c\'%\x90\x9c\'&\x12\xc2\x01\n\x0b\x44\x65leteTasks\x12 .clarifai.api.DeleteTasksRequest\x1a!.clarifai.api.status.BaseResponse\"n\x82\xd3\xe4\x93\x02T*?/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks:\x01*Z\x0e*\t/v2/tasks:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xf5\x01\n\x0fPostLabelOrders\x12$.clarifai.api.PostLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x94\x01\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\"\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x90\x9c\'\x05\x90\x9c\'r\x90\x9c\'\x0b\x90\x9c\'\x13\x90\x9c\'\x0f\x12\xf6\x01\n\rGetLabelOrder\x12\".clarifai.api.GetLabelOrderRequest\x1a&.clarifai.api.SingleLabelOrderResponse\"\x98\x01\x82\xd3\xe4\x93\x02~\x12W/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders/{label_order_id}Z#\x12!/v2/label_orders/{label_order_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xd6\x01\n\x0fListLabelOrders\x12$.clarifai.api.ListLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"v\x82\xd3\xe4\x93\x02\\\x12\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_ordersZ\x12\x12\x10/v2/label_orders\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'\x0b\x90\x9c\'8\x12\xeb\x01\n\x10PatchLabelOrders\x12%.clarifai.api.PatchLabelOrdersRequest\x1a%.clarifai.api.MultiLabelOrderResponse\"\x88\x01\x82\xd3\xe4\x93\x02\x62\x32\x46/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15\x32\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'C\x90\x9c\'D\x90\x9c\'\x0b\x90\x9c\'7\x90\x9c\'8\x90\x9c\'F\x12\xe5\x01\n\x11\x44\x65leteLabelOrders\x12&.clarifai.api.DeleteLabelOrdersRequest\x1a!.clarifai.api.status.BaseResponse\"\x84\x01\x82\xd3\xe4\x93\x02\x62*F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/label_orders:\x01*Z\x15*\x10/v2/label_orders:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'E\x90\x9c\'C\x90\x9c\'D\x90\x9c\'7\x90\x9c\'8\x12\xf2\x01\n\x0ePostCollectors\x12#.clarifai.api.PostCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"\x94\x01\x82\xd3\xe4\x93\x02^\"D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\"\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'%\x90\x9c\'&\x90\x9c\')\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xe3\x01\n\x0cGetCollector\x12!.clarifai.api.GetCollectorRequest\x1a%.clarifai.api.SingleCollectorResponse\"\x88\x01\x82\xd3\xe4\x93\x02v\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors/{collector_id}Z\x1f\x12\x1d/v2/collectors/{collector_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'*\x12\xc7\x01\n\x0eListCollectors\x12#.clarifai.api.ListCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"j\x82\xd3\xe4\x93\x02X\x12\x44/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectorsZ\x10\x12\x0e/v2/collectors\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'*\x12\xd3\x01\n\x0fPatchCollectors\x12$.clarifai.api.PatchCollectorsRequest\x1a$.clarifai.api.MultiCollectorResponse\"t\x82\xd3\xe4\x93\x02^2D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13\x32\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\')\x90\x9c\'*\x12\xd6\x01\n\x10\x44\x65leteCollectors\x12%.clarifai.api.DeleteCollectorsRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02^*D/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/collectors:\x01*Z\x13*\x0e/v2/collectors:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\')\x90\x9c\'+\x90\x9c\'*\x12\xc9\x01\n\x0ePostStatValues\x12#.clarifai.api.PostStatValuesRequest\x1a$.clarifai.api.MultiStatValueResponse\"l\x82\xd3\xe4\x93\x02\x62\"F/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values:\x01*Z\x15\"\x10/v2/stats/values:\x01*\x98\x9c\'\x02\x12\xfd\x01\n\x17PostStatValuesAggregate\x12,.clarifai.api.PostStatValuesAggregateRequest\x1a-.clarifai.api.MultiStatValueAggregateResponse\"\x84\x01\x82\xd3\xe4\x93\x02v\"P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/stats/values/aggregate:\x01*Z\x1f\"\x1a/v2/stats/values/aggregate:\x01*\x98\x9c\'\x02\x90\x9c\'-\x12\xe3\x01\n\x17PostTrendingMetricsView\x12,.clarifai.api.PostTrendingMetricsViewRequest\x1a!.clarifai.api.status.BaseResponse\"w\x82\xd3\xe4\x93\x02m\"h/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}/{object_id}:\x01*\x98\x9c\'\x02\x12\x8f\x02\n\x18ListTrendingMetricsViews\x12-.clarifai.api.ListTrendingMetricsViewsRequest\x1a..clarifai.api.MultiTrendingMetricsViewResponse\"\x93\x01\x82\xd3\xe4\x93\x02\x88\x01\x12\\/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/trending_metrics/views/{view_type}Z(\x12&/v2/trending_metrics/views/{view_type}\x98\x9c\'\x02\x12\xb2\x01\n\tGetModule\x12\x1e.clarifai.api.GetModuleRequest\x1a\".clarifai.api.SingleModuleResponse\"a\x82\xd3\xe4\x93\x02O\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xe4\x01\n\x0bListModules\x12 .clarifai.api.ListModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\x8f\x01\x82\xd3\xe4\x93\x02}\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modulesZ)\x12\'/v2/users/{user_app_id.user_id}/modulesZ\r\x12\x0b/v2/modules\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xb0\x01\n\x0bPostModules\x12 .clarifai.api.PostModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\\\x82\xd3\xe4\x93\x02\x46\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xb2\x01\n\x0cPatchModules\x12!.clarifai.api.PatchModulesRequest\x1a!.clarifai.api.MultiModuleResponse\"\\\x82\xd3\xe4\x93\x02\x46\x32\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xd0\x01\n\rDeleteModules\x12\".clarifai.api.DeleteModulesRequest\x1a!.clarifai.api.status.BaseResponse\"x\x82\xd3\xe4\x93\x02\x46*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x90\x9c\'p\x90\x9c\'o\x90\x9c\'q\x90\x9c\'1\x90\x9c\'0\x90\x9c\'/\x12\xe4\x01\n\x10GetModuleVersion\x12%.clarifai.api.GetModuleVersionRequest\x1a).clarifai.api.SingleModuleVersionResponse\"~\x82\xd3\xe4\x93\x02l\x12j/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions/{module_version_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xd3\x01\n\x12ListModuleVersions\x12\'.clarifai.api.ListModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"j\x82\xd3\xe4\x93\x02X\x12V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x12\xda\x01\n\x12PostModuleVersions\x12\'.clarifai.api.PostModuleVersionsRequest\x1a(.clarifai.api.MultiModuleVersionResponse\"q\x82\xd3\xe4\x93\x02[\"V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'m\x12\xf4\x01\n\x14\x44\x65leteModuleVersions\x12).clarifai.api.DeleteModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x8d\x01\x82\xd3\xe4\x93\x02[*V/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/modules/{module_id}/versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'l\x90\x9c\'n\x90\x9c\'m\x90\x9c\'p\x90\x9c\'o\x90\x9c\'q\x90\x9c\'1\x90\x9c\'0\x90\x9c\'/\x12\x8f\x02\n\x19GetInstalledModuleVersion\x12..clarifai.api.GetInstalledModuleVersionRequest\x1a\x32.clarifai.api.SingleInstalledModuleVersionResponse\"\x8d\x01\x82\xd3\xe4\x93\x02s\x12q/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf3\x01\n\x1bListInstalledModuleVersions\x12\x30.clarifai.api.ListInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"o\x82\xd3\xe4\x93\x02U\x12S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'p\x90\x9c\'m\x90\x9c\'0\x12\xf6\x01\n\x1bPostInstalledModuleVersions\x12\x30.clarifai.api.PostInstalledModuleVersionsRequest\x1a\x31.clarifai.api.MultiInstalledModuleVersionResponse\"r\x82\xd3\xe4\x93\x02X\"S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x12\xfb\x01\n\x1d\x44\x65leteInstalledModuleVersions\x12\x32.clarifai.api.DeleteInstalledModuleVersionsRequest\x1a!.clarifai.api.status.BaseResponse\"\x82\x01\x82\xd3\xe4\x93\x02X*S/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'m\x90\x9c\'o\x90\x9c\'p\x90\x9c\'q\x90\x9c\'1\x90\x9c\'/\x90\x9c\'0\x12\x95\x02\n\x1ePostInstalledModuleVersionsKey\x12\x33.clarifai.api.PostInstalledModuleVersionsKeyRequest\x1a\x1f.clarifai.api.SingleKeyResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\"u/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/installed_module_versions/{installed_module_version_id}/key:\x01*\x98\x9c\'\x05\x90\x9c\'o\x90\x9c\'p\x90\x9c\'m\x90\x9c\'-\x90\x9c\'/\x90\x9c\'0\x12\xf5\x01\n\x12PostBulkOperations\x12\'.clarifai.api.PostBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"\x8a\x01\x82\xd3\xe4\x93\x02h\"I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\"\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x90\x9c\'y\x90\x9c\'%\x90\x9c\'&\x90\x9c\'(\x12\xde\x01\n\x12ListBulkOperations\x12\'.clarifai.api.ListBulkOperationsRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"t\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operationsZ\x15\x12\x13/v2/bulk_operations\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x12\xe5\x01\n\x10GetBulkOperation\x12%.clarifai.api.GetBulkOperationRequest\x1a*.clarifai.api.SingleBulkOperationsResponse\"~\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations/{id}Z\x1a\x12\x18/v2/bulk_operations/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'z\x12\xeb\x01\n\x14\x43\x61ncelBulkOperations\x12(.clarifai.api.CancelBulkOperationRequest\x1a).clarifai.api.MultiBulkOperationsResponse\"~\x82\xd3\xe4\x93\x02h2I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18\x32\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'y\x90\x9c\'z\x12\xf4\x01\n\x14\x44\x65leteBulkOperations\x12(.clarifai.api.DeleteBulkOperationRequest\x1a!.clarifai.api.status.BaseResponse\"\x8e\x01\x82\xd3\xe4\x93\x02h*I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/bulk_operations:\x01*Z\x18*\x13/v2/bulk_operations:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'%\x90\x9c\'(\x90\x9c\'y\x90\x9c\'z\x90\x9c\'{\x12\xb2\x02\n\x1cGetDatasetInputsSearchAddJob\x12\x31.clarifai.api.GetDatasetInputsSearchAddJobRequest\x1a\x35.clarifai.api.SingleDatasetInputsSearchAddJobResponse\"\xa7\x01\x82\xd3\xe4\x93\x02\x94\x01\x12\x62/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/datasets/inputs/search_add/jobs/{job_id}Z.\x12,/v2/datasets/inputs/search_add/jobs/{job_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'i\x12\x88\x02\n\x17ListNextTaskAssignments\x12,.clarifai.api.ListNextTaskAssignmentsRequest\x1a .clarifai.api.MultiInputResponse\"\x9c\x01\x82\xd3\xe4\x93\x02z\x12U/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignmentsZ!\x12\x1f/v2/tasks/{task_id}/assignments\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xe3\x01\n\x12PutTaskAssignments\x12\'.clarifai.api.PutTaskAssignmentsRequest\x1a!.clarifai.api.status.BaseResponse\"\x80\x01\x82\xd3\xe4\x93\x02Z\x1aU/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/tasks/{task_id}/assignments:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x05\x90\x9c\'8\x90\x9c\'i\x12\xda\x01\n\x11ListInputsAddJobs\x12&.clarifai.api.ListInputsAddJobsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"t\x82\xd3\xe4\x93\x02\x62\x12I/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/addZ\x15\x12\x13/v2/inputs/jobs/add\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xe1\x01\n\x0fGetInputsAddJob\x12$.clarifai.api.GetInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"~\x82\xd3\xe4\x93\x02l\x12N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}Z\x1a\x12\x18/v2/inputs/jobs/add/{id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xf2\x01\n\x12\x43\x61ncelInputsAddJob\x12\'.clarifai.api.CancelInputsAddJobRequest\x1a(.clarifai.api.SingleInputsAddJobResponse\"\x88\x01\x82\xd3\xe4\x93\x02r2N/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/add/{id}:\x01*Z\x1d\x32\x18/v2/inputs/jobs/add/{id}:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'\x05\x12\xc4\x01\n\x0bPostUploads\x12 .clarifai.api.PostUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"p\x82\xd3\xe4\x93\x02X\"A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10\"\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\x8c\x02\n\x15PutUploadContentParts\x12*.clarifai.api.PutUploadContentPartsRequest\x1a\".clarifai.api.SingleUploadResponse\"\xa2\x01\x82\xd3\xe4\x93\x02\x89\x01\x1a[/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}/content_parts:\x01*Z\'\x1a%/v2/uploads/{upload_id}/content_parts\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\xce\x01\n\tGetUpload\x12\x1e.clarifai.api.GetUploadRequest\x1a\".clarifai.api.SingleUploadResponse\"}\x82\xd3\xe4\x93\x02j\x12M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads/{upload_id}Z\x19\x12\x17/v2/uploads/{upload_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x12\xb9\x01\n\x0bListUploads\x12 .clarifai.api.ListUploadsRequest\x1a!.clarifai.api.MultiUploadResponse\"e\x82\xd3\xe4\x93\x02R\x12\x41/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploadsZ\r\x12\x0b/v2/uploads\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x12\xcd\x01\n\rDeleteUploads\x12\".clarifai.api.DeleteUploadsRequest\x1a!.clarifai.api.status.BaseResponse\"u\x82\xd3\xe4\x93\x02X*A/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/uploads:\x01*Z\x10*\x0b/v2/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x80\x01\x90\x9c\'\x81\x01\x90\x9c\'\x82\x01\x12\x8d\x02\n\x15PostInputsDataSources\x12*.clarifai.api.PostInputsDataSourcesRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9e\x01\x82\xd3\xe4\x93\x02p\"M/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/data_sources:\x01*Z\x1c\"\x17/v2/inputs/data_sources:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x12\xb2\x02\n\x16GetInputsExtractionJob\x12+.clarifai.api.GetInputsExtractionJobRequest\x1a/.clarifai.api.SingleInputsExtractionJobResponse\"\xb9\x01\x82\xd3\xe4\x93\x02\xa6\x01\x12k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\x12\x35/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\xfe\x01\n\x18ListInputsExtractionJobs\x12-.clarifai.api.ListInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x82\x01\x82\xd3\xe4\x93\x02p\x12P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\x1c\x12\x1a/v2/inputs/jobs/extraction\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x05\x12\x8c\x02\n\x1a\x43\x61ncelInputsExtractionJobs\x12/.clarifai.api.CancelInputsExtractionJobsRequest\x1a..clarifai.api.MultiInputsExtractionJobResponse\"\x8c\x01\x82\xd3\xe4\x93\x02v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\x01*Z\x1f\x32\x1a/v2/inputs/jobs/extraction:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'\x04\x90\x9c\'\x05\x12\x85\x02\n\x11PostInputsUploads\x12&.clarifai.api.PostInputsUploadsRequest\x1a\'.clarifai.api.MultiInputsAddJobResponse\"\x9e\x01\x82\xd3\xe4\x93\x02\x66\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\x01*Z\x17\"\x12/v2/inputs/uploads:\x01*\x98\x9c\'\x02\x90\x9c\'-\x90\x9c\'%\x90\x9c\'&\x90\x9c\'\x0b\x90\x9c\'\x04\x90\x9c\'\x05\x90\x9c\'\x0f\x90\x9c\'\x02\x90\x9c\'\x13\x90\x9c\'\x81\x01\x90\x9c\'\x80\x01\x12\x99\x01\n\tGetRunner\x12\x1e.clarifai.api.GetRunnerRequest\x1a\".clarifai.api.SingleRunnerResponse\"H\x82\xd3\xe4\x93\x02\x35\x12\x33/v2/users/{user_app_id.user_id}/runners/{runner_id}\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x83\x01\x12\x90\x01\n\x0bListRunners\x12 .clarifai.api.ListRunnersRequest\x1a!.clarifai.api.MultiRunnerResponse\"<\x82\xd3\xe4\x93\x02)\x12\'/v2/users/{user_app_id.user_id}/runners\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x83\x01\x12\x98\x01\n\x0bPostRunners\x12 .clarifai.api.PostRunnersRequest\x1a!.clarifai.api.MultiRunnerResponse\"D\x82\xd3\xe4\x93\x02,\"\'/v2/users/{user_app_id.user_id}/runners:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x83\x01\x90\x9c\'\x84\x01\x12\xa1\x01\n\rDeleteRunners\x12\".clarifai.api.DeleteRunnersRequest\x1a!.clarifai.api.status.BaseResponse\"I\x82\xd3\xe4\x93\x02,*\'/v2/users/{user_app_id.user_id}/runners:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x83\x01\x90\x9c\'\x84\x01\x90\x9c\'\x85\x01\x12\xb3\x01\n\x0fListRunnerItems\x12$.clarifai.api.ListRunnerItemsRequest\x1a%.clarifai.api.MultiRunnerItemResponse\"S\x82\xd3\xe4\x93\x02;\x12\x39/v2/users/{user_app_id.user_id}/runners/{runner_id}/items\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x83\x01\x90\x9c\'\x86\x01\x12\xdf\x01\n\x15PostRunnerItemOutputs\x12*.clarifai.api.PostRunnerItemOutputsRequest\x1a+.clarifai.api.MultiRunnerItemOutputResponse\"m\x82\xd3\xe4\x93\x02P\"K/v2/users/{user_app_id.user_id}/runners/{runner_id}/items/{item_id}/outputs:\x01*\x98\x9c\'\x05\x90\x9c\'-\x90\x9c\'\x83\x01\x90\x9c\'\x86\x01\x90\x9c\'\x87\x01\x42Y\n\x15\x63om.clarifai.grpc.apiP\x01Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025com.clarifai.grpc.apiP\001Z7github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api\242\002\004CAIP'
@@ -101,14 +101,20 @@
   _MULTIMODULERESPONSE.fields_by_name['modules']._serialized_options = b'\200\265\030\001'
   _MULTIMODULEVERSIONRESPONSE.fields_by_name['module_versions']._options = None
   _MULTIMODULEVERSIONRESPONSE.fields_by_name['module_versions']._serialized_options = b'\200\265\030\001'
   _MULTIINSTALLEDMODULEVERSIONRESPONSE.fields_by_name['installed_module_versions']._options = None
   _MULTIINSTALLEDMODULEVERSIONRESPONSE.fields_by_name['installed_module_versions']._serialized_options = b'\200\265\030\001'
   _MULTIINPUTSADDJOBRESPONSE.fields_by_name['inputs_add_jobs']._options = None
   _MULTIINPUTSADDJOBRESPONSE.fields_by_name['inputs_add_jobs']._serialized_options = b'\200\265\030\001'
+  _MULTIRUNNERRESPONSE.fields_by_name['runners']._options = None
+  _MULTIRUNNERRESPONSE.fields_by_name['runners']._serialized_options = b'\200\265\030\001'
+  _MULTIRUNNERITEMRESPONSE.fields_by_name['items']._options = None
+  _MULTIRUNNERITEMRESPONSE.fields_by_name['items']._serialized_options = b'\200\265\030\001'
+  _MULTIRUNNERITEMOUTPUTRESPONSE.fields_by_name['runner_item_outputs']._options = None
+  _MULTIRUNNERITEMOUTPUTRESPONSE.fields_by_name['runner_item_outputs']._serialized_options = b'\200\265\030\001'
   _V2.methods_by_name['ListConceptRelations']._options = None
   _V2.methods_by_name['ListConceptRelations']._serialized_options = b'\202\323\344\223\002\253\001\022Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relationsZN\022L/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/relations\230\234\'\005\220\234\'-\220\234\'\013'
   _V2.methods_by_name['PostConceptRelations']._options = None
   _V2.methods_by_name['PostConceptRelations']._serialized_options = b'\202\323\344\223\002^\"Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\001*\230\234\'\005\220\234\'-\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['DeleteConceptRelations']._options = None
   _V2.methods_by_name['DeleteConceptRelations']._serialized_options = b'\202\323\344\223\002^*Y/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/concepts/{concept_id}/relations:\001*\230\234\'\005\220\234\'-\220\234\'\r\220\234\'\n\220\234\'\013'
   _V2.methods_by_name['GetConceptCounts']._options = None
@@ -515,16 +521,28 @@
   _V2.methods_by_name['GetInputsExtractionJob']._serialized_options = b'\202\323\344\223\002\246\001\022k/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction/{inputs_extraction_job_id}Z7\0225/v2/inputs/jobs/extraction/{inputs_extraction_job_id}\230\234\'\002\220\234\'-\220\234\'\005'
   _V2.methods_by_name['ListInputsExtractionJobs']._options = None
   _V2.methods_by_name['ListInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002p\022P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extractionZ\034\022\032/v2/inputs/jobs/extraction\230\234\'\002\220\234\'-\220\234\'\005'
   _V2.methods_by_name['CancelInputsExtractionJobs']._options = None
   _V2.methods_by_name['CancelInputsExtractionJobs']._serialized_options = b'\202\323\344\223\002v2P/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/jobs/extraction:\001*Z\0372\032/v2/inputs/jobs/extraction:\001*\230\234\'\002\220\234\'-\220\234\'\004\220\234\'\005'
   _V2.methods_by_name['PostInputsUploads']._options = None
   _V2.methods_by_name['PostInputsUploads']._serialized_options = b'\202\323\344\223\002f\"H/v2/users/{user_app_id.user_id}/apps/{user_app_id.app_id}/inputs/uploads:\001*Z\027\"\022/v2/inputs/uploads:\001*\230\234\'\002\220\234\'-\220\234\'%\220\234\'&\220\234\'\013\220\234\'\004\220\234\'\005\220\234\'\017\220\234\'\002\220\234\'\023\220\234\'\201\001\220\234\'\200\001'
-  _ORGANIZATIONINVITATIONSTATUS._serialized_start=40733
-  _ORGANIZATIONINVITATIONSTATUS._serialized_end=40845
+  _V2.methods_by_name['GetRunner']._options = None
+  _V2.methods_by_name['GetRunner']._serialized_options = b'\202\323\344\223\0025\0223/v2/users/{user_app_id.user_id}/runners/{runner_id}\230\234\'\005\220\234\'-\220\234\'\203\001'
+  _V2.methods_by_name['ListRunners']._options = None
+  _V2.methods_by_name['ListRunners']._serialized_options = b'\202\323\344\223\002)\022\'/v2/users/{user_app_id.user_id}/runners\230\234\'\005\220\234\'-\220\234\'\203\001'
+  _V2.methods_by_name['PostRunners']._options = None
+  _V2.methods_by_name['PostRunners']._serialized_options = b'\202\323\344\223\002,\"\'/v2/users/{user_app_id.user_id}/runners:\001*\230\234\'\005\220\234\'-\220\234\'\203\001\220\234\'\204\001'
+  _V2.methods_by_name['DeleteRunners']._options = None
+  _V2.methods_by_name['DeleteRunners']._serialized_options = b'\202\323\344\223\002,*\'/v2/users/{user_app_id.user_id}/runners:\001*\230\234\'\005\220\234\'-\220\234\'\203\001\220\234\'\204\001\220\234\'\205\001'
+  _V2.methods_by_name['ListRunnerItems']._options = None
+  _V2.methods_by_name['ListRunnerItems']._serialized_options = b'\202\323\344\223\002;\0229/v2/users/{user_app_id.user_id}/runners/{runner_id}/items\230\234\'\005\220\234\'-\220\234\'\203\001\220\234\'\206\001'
+  _V2.methods_by_name['PostRunnerItemOutputs']._options = None
+  _V2.methods_by_name['PostRunnerItemOutputs']._serialized_options = b'\202\323\344\223\002P\"K/v2/users/{user_app_id.user_id}/runners/{runner_id}/items/{item_id}/outputs:\001*\230\234\'\005\220\234\'-\220\234\'\203\001\220\234\'\206\001\220\234\'\207\001'
+  _ORGANIZATIONINVITATIONSTATUS._serialized_start=42590
+  _ORGANIZATIONINVITATIONSTATUS._serialized_end=42702
   _PAGINATION._serialized_start=420
   _PAGINATION._serialized_end=464
   _GETANNOTATIONREQUEST._serialized_start=466
   _GETANNOTATIONREQUEST._serialized_end=578
   _LISTANNOTATIONSREQUEST._serialized_start=581
   _LISTANNOTATIONSREQUEST._serialized_end=892
   _POSTANNOTATIONSREQUEST._serialized_start=894
@@ -542,595 +560,619 @@
   _SINGLEANNOTATIONRESPONSE._serialized_start=1720
   _SINGLEANNOTATIONRESPONSE._serialized_end=1837
   _MULTIANNOTATIONRESPONSE._serialized_start=1839
   _MULTIANNOTATIONRESPONSE._serialized_end=1962
   _GETAPPREQUEST._serialized_start=1964
   _GETAPPREQUEST._serialized_end=2055
   _LISTAPPSREQUEST._serialized_start=2058
-  _LISTAPPSREQUEST._serialized_end=2351
-  _POSTAPPSREQUEST._serialized_start=2353
-  _POSTAPPSREQUEST._serialized_end=2452
-  _DELETEAPPREQUEST._serialized_start=2454
-  _DELETEAPPREQUEST._serialized_end=2521
-  _PATCHAPPSREQUEST._serialized_start=2524
-  _PATCHAPPSREQUEST._serialized_end=2709
-  _PATCHAPPREQUEST._serialized_start=2712
-  _PATCHAPPREQUEST._serialized_end=2895
-  _PATCHAPPSIDSREQUEST._serialized_start=2898
-  _PATCHAPPSIDSREQUEST._serialized_end=3027
-  _POSTAPPSSEARCHESREQUEST._serialized_start=3030
-  _POSTAPPSSEARCHESREQUEST._serialized_end=3193
-  _SINGLEAPPRESPONSE._serialized_start=3195
-  _SINGLEAPPRESPONSE._serialized_end=3291
-  _MULTIAPPRESPONSE._serialized_start=3293
-  _MULTIAPPRESPONSE._serialized_end=3395
-  _LISTCOLLABORATORSREQUEST._serialized_start=3398
-  _LISTCOLLABORATORSREQUEST._serialized_end=3537
-  _POSTCOLLABORATORSREQUEST._serialized_start=3539
-  _POSTCOLLABORATORSREQUEST._serialized_end=3665
-  _PATCHCOLLABORATORSREQUEST._serialized_start=3668
-  _PATCHCOLLABORATORSREQUEST._serialized_end=3811
-  _DELETECOLLABORATORSREQUEST._serialized_start=3813
-  _DELETECOLLABORATORSREQUEST._serialized_end=3937
-  _MULTICOLLABORATORSRESPONSE._serialized_start=3940
-  _MULTICOLLABORATORSRESPONSE._serialized_end=4070
-  _LISTCOLLABORATIONSREQUEST._serialized_start=4072
-  _LISTCOLLABORATIONSREQUEST._serialized_end=4180
-  _MULTICOLLABORATIONSRESPONSE._serialized_start=4183
-  _MULTICOLLABORATIONSRESPONSE._serialized_end=4316
-  _GETSTATUSCODEREQUEST._serialized_start=4318
-  _GETSTATUSCODEREQUEST._serialized_end=4364
-  _LISTSTATUSCODESREQUEST._serialized_start=4366
-  _LISTSTATUSCODESREQUEST._serialized_end=4390
-  _SINGLESTATUSCODERESPONSE._serialized_start=4392
-  _SINGLESTATUSCODERESPONSE._serialized_end=4463
-  _MULTISTATUSCODERESPONSE._serialized_start=4465
-  _MULTISTATUSCODERESPONSE._serialized_end=4582
-  _GETCONCEPTREQUEST._serialized_start=4584
-  _GETCONCEPTREQUEST._serialized_end=4672
-  _LISTCONCEPTSREQUEST._serialized_start=4674
-  _LISTCONCEPTSREQUEST._serialized_end=4776
-  _LISTMODELCONCEPTSREQUEST._serialized_start=4779
-  _LISTMODELCONCEPTSREQUEST._serialized_end=4924
-  _POSTCONCEPTSSEARCHESREQUEST._serialized_start=4927
-  _POSTCONCEPTSSEARCHESREQUEST._serialized_end=5102
-  _POSTCONCEPTSREQUEST._serialized_start=5104
-  _POSTCONCEPTSREQUEST._serialized_end=5215
-  _PATCHCONCEPTSREQUEST._serialized_start=5218
-  _PATCHCONCEPTSREQUEST._serialized_end=5346
-  _GETCONCEPTCOUNTSREQUEST._serialized_start=5348
-  _GETCONCEPTCOUNTSREQUEST._serialized_end=5454
-  _SINGLECONCEPTRESPONSE._serialized_start=5456
-  _SINGLECONCEPTRESPONSE._serialized_end=5564
-  _MULTICONCEPTRESPONSE._serialized_start=5566
-  _MULTICONCEPTRESPONSE._serialized_end=5680
-  _MULTICONCEPTCOUNTRESPONSE._serialized_start=5683
-  _MULTICONCEPTCOUNTRESPONSE._serialized_end=5813
-  _LISTCONCEPTRELATIONSREQUEST._serialized_start=5816
-  _LISTCONCEPTRELATIONSREQUEST._serialized_end=5993
-  _POSTCONCEPTRELATIONSREQUEST._serialized_start=5996
-  _POSTCONCEPTRELATIONSREQUEST._serialized_end=6152
-  _DELETECONCEPTRELATIONSREQUEST._serialized_start=6154
-  _DELETECONCEPTRELATIONSREQUEST._serialized_end=6267
-  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_start=6269
-  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_end=6346
-  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_start=6349
-  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_end=6482
-  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_start=6485
-  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_end=6628
-  _MULTICONCEPTRELATIONRESPONSE._serialized_start=6631
-  _MULTICONCEPTRELATIONRESPONSE._serialized_end=6770
-  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_start=6773
-  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_end=6909
-  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_start=6911
-  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_end=7001
-  _GETCONCEPTLANGUAGEREQUEST._serialized_start=7003
-  _GETCONCEPTLANGUAGEREQUEST._serialized_end=7117
-  _LISTCONCEPTLANGUAGESREQUEST._serialized_start=7120
-  _LISTCONCEPTLANGUAGESREQUEST._serialized_end=7250
-  _PATCHCONCEPTLANGUAGESREQUEST._serialized_start=7253
-  _PATCHCONCEPTLANGUAGESREQUEST._serialized_end=7426
-  _POSTCONCEPTLANGUAGESREQUEST._serialized_start=7429
-  _POSTCONCEPTLANGUAGESREQUEST._serialized_end=7585
-  _SINGLECONCEPTLANGUAGERESPONSE._serialized_start=7588
-  _SINGLECONCEPTLANGUAGERESPONSE._serialized_end=7721
-  _MULTICONCEPTLANGUAGERESPONSE._serialized_start=7724
-  _MULTICONCEPTLANGUAGERESPONSE._serialized_end=7863
-  _GETINPUTREQUEST._serialized_start=7865
-  _GETINPUTREQUEST._serialized_end=7949
-  _GETVIDEOMANIFESTREQUEST._serialized_start=7951
-  _GETVIDEOMANIFESTREQUEST._serialized_end=8043
-  _GETINPUTSAMPLESREQUEST._serialized_start=8045
-  _GETINPUTSAMPLESREQUEST._serialized_end=8153
-  _LISTINPUTSREQUEST._serialized_start=8156
-  _LISTINPUTSREQUEST._serialized_end=8314
-  _STREAMINPUTSREQUEST._serialized_start=8317
-  _STREAMINPUTSREQUEST._serialized_end=8463
-  _POSTINPUTSREQUEST._serialized_start=8466
-  _POSTINPUTSREQUEST._serialized_end=8677
-  _PATCHINPUTSREQUEST._serialized_start=8679
-  _PATCHINPUTSREQUEST._serialized_end=8801
-  _DELETEINPUTREQUEST._serialized_start=8803
-  _DELETEINPUTREQUEST._serialized_end=8890
-  _DELETEINPUTSREQUEST._serialized_start=8892
-  _DELETEINPUTSREQUEST._serialized_end=8981
-  _SINGLEINPUTRESPONSE._serialized_start=8983
-  _SINGLEINPUTRESPONSE._serialized_end=9085
-  _GETVIDEOMANIFESTRESPONSE._serialized_start=9087
-  _GETVIDEOMANIFESTRESPONSE._serialized_end=9180
-  _MULTIINPUTRESPONSE._serialized_start=9183
-  _MULTIINPUTRESPONSE._serialized_end=9343
-  _MULTIINPUTANNOTATIONRESPONSE._serialized_start=9345
-  _MULTIINPUTANNOTATIONRESPONSE._serialized_end=9459
-  _SINGLEINPUTCOUNTRESPONSE._serialized_start=9461
-  _SINGLEINPUTCOUNTRESPONSE._serialized_end=9574
-  _GETINPUTCOUNTREQUEST._serialized_start=9576
-  _GETINPUTCOUNTREQUEST._serialized_end=9647
-  _LISTDATASETSREQUEST._serialized_start=9650
-  _LISTDATASETSREQUEST._serialized_end=9801
-  _GETDATASETREQUEST._serialized_start=9803
-  _GETDATASETREQUEST._serialized_end=9918
-  _POSTDATASETSREQUEST._serialized_start=9920
-  _POSTDATASETSREQUEST._serialized_end=10031
-  _PATCHDATASETSREQUEST._serialized_start=10034
-  _PATCHDATASETSREQUEST._serialized_end=10162
-  _DELETEDATASETSREQUEST._serialized_start=10164
-  _DELETEDATASETSREQUEST._serialized_end=10257
-  _MULTIDATASETRESPONSE._serialized_start=10259
-  _MULTIDATASETRESPONSE._serialized_end=10373
-  _SINGLEDATASETRESPONSE._serialized_start=10375
-  _SINGLEDATASETRESPONSE._serialized_end=10483
-  _LISTDATASETINPUTSREQUEST._serialized_start=10485
-  _LISTDATASETINPUTSREQUEST._serialized_end=10612
-  _GETDATASETINPUTREQUEST._serialized_start=10614
-  _GETDATASETINPUTREQUEST._serialized_end=10725
-  _POSTDATASETINPUTSREQUEST._serialized_start=10728
-  _POSTDATASETINPUTSREQUEST._serialized_end=10913
-  _DELETEDATASETINPUTSREQUEST._serialized_start=10915
-  _DELETEDATASETINPUTSREQUEST._serialized_end=11031
-  _MULTIDATASETINPUTRESPONSE._serialized_start=11034
-  _MULTIDATASETINPUTRESPONSE._serialized_end=11244
-  _SINGLEDATASETINPUTRESPONSE._serialized_start=11246
-  _SINGLEDATASETINPUTRESPONSE._serialized_end=11370
-  _LISTDATASETVERSIONSREQUEST._serialized_start=11373
-  _LISTDATASETVERSIONSREQUEST._serialized_end=11502
-  _GETDATASETVERSIONREQUEST._serialized_start=11504
-  _GETDATASETVERSIONREQUEST._serialized_end=11627
-  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_start=11630
-  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_end=11922
-  _POSTDATASETVERSIONSREQUEST._serialized_start=11925
-  _POSTDATASETVERSIONSREQUEST._serialized_end=12078
-  _PATCHDATASETVERSIONSREQUEST._serialized_start=12081
-  _PATCHDATASETVERSIONSREQUEST._serialized_end=12251
-  _DELETEDATASETVERSIONSREQUEST._serialized_start=12254
-  _DELETEDATASETVERSIONSREQUEST._serialized_end=12382
-  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_start=12385
-  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_end=12568
-  _MULTIDATASETVERSIONRESPONSE._serialized_start=12571
-  _MULTIDATASETVERSIONRESPONSE._serialized_end=12707
-  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_start=12710
-  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_end=12849
-  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_start=12852
-  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_end=13026
-  _SINGLEDATASETVERSIONRESPONSE._serialized_start=13029
-  _SINGLEDATASETVERSIONRESPONSE._serialized_end=13159
-  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_start=13161
-  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_end=13263
-  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_start=13266
-  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_end=13406
-  _POSTMODELOUTPUTSREQUEST._serialized_start=13409
-  _POSTMODELOUTPUTSREQUEST._serialized_end=13594
-  _LISTMODELINPUTSREQUEST._serialized_start=13597
-  _LISTMODELINPUTSREQUEST._serialized_end=13740
-  _GETKEYREQUEST._serialized_start=13742
-  _GETKEYREQUEST._serialized_end=13822
-  _LISTKEYSREQUEST._serialized_start=13825
-  _LISTKEYSREQUEST._serialized_end=13979
-  _LISTAPPKEYSREQUEST._serialized_start=13981
-  _LISTAPPKEYSREQUEST._serialized_end=14082
-  _POSTKEYSREQUEST._serialized_start=14084
-  _POSTKEYSREQUEST._serialized_end=14183
-  _DELETEKEYREQUEST._serialized_start=14185
-  _DELETEKEYREQUEST._serialized_end=14268
-  _PATCHKEYSREQUEST._serialized_start=14270
-  _PATCHKEYSREQUEST._serialized_end=14386
-  _SINGLEKEYRESPONSE._serialized_start=14388
-  _SINGLEKEYRESPONSE._serialized_end=14484
-  _MULTIKEYRESPONSE._serialized_start=14486
-  _MULTIKEYRESPONSE._serialized_end=14588
-  _GETMODELREQUEST._serialized_start=14591
-  _GETMODELREQUEST._serialized_end=14764
-  _LISTMODELSREQUEST._serialized_start=14767
-  _LISTMODELSREQUEST._serialized_end=15314
-  _GETRESOURCECOUNTSREQUEST._serialized_start=15316
-  _GETRESOURCECOUNTSREQUEST._serialized_end=15391
-  _GETRESOURCECOUNTSRESPONSE._serialized_start=15394
-  _GETRESOURCECOUNTSRESPONSE._serialized_end=15536
-  _PATCHMODELTOOLKITSREQUEST._serialized_start=15539
-  _PATCHMODELTOOLKITSREQUEST._serialized_end=15667
-  _PATCHMODELCHECKCONSENTSREQUEST._serialized_start=15670
-  _PATCHMODELCHECKCONSENTSREQUEST._serialized_end=15809
-  _PATCHMODELUSECASESREQUEST._serialized_start=15812
-  _PATCHMODELUSECASESREQUEST._serialized_end=15940
-  _PATCHMODELLANGUAGESREQUEST._serialized_start=15943
-  _PATCHMODELLANGUAGESREQUEST._serialized_end=16073
-  _MULTIMODELTOOLKITRESPONSE._serialized_start=16075
-  _MULTIMODELTOOLKITRESPONSE._serialized_end=16165
-  _MULTIMODELCHECKCONSENTRESPONSE._serialized_start=16167
-  _MULTIMODELCHECKCONSENTRESPONSE._serialized_end=16268
-  _MULTIMODELUSECASERESPONSE._serialized_start=16270
-  _MULTIMODELUSECASERESPONSE._serialized_end=16360
-  _MULTIMODELLANGUAGERESPONSE._serialized_start=16362
-  _MULTIMODELLANGUAGERESPONSE._serialized_end=16454
-  _POSTMODELSREQUEST._serialized_start=16457
-  _POSTMODELSREQUEST._serialized_end=16602
-  _PATCHMODELSREQUEST._serialized_start=16604
-  _PATCHMODELSREQUEST._serialized_end=16726
-  _IDUPDATESOURCE._serialized_start=16728
-  _IDUPDATESOURCE._serialized_end=16772
-  _PATCHMODELIDSREQUEST._serialized_start=16775
-  _PATCHMODELIDSREQUEST._serialized_end=16905
-  _DELETEMODELREQUEST._serialized_start=16907
-  _DELETEMODELREQUEST._serialized_end=16994
-  _DELETEMODELSREQUEST._serialized_start=16996
-  _DELETEMODELSREQUEST._serialized_end=17099
-  _POSTMODELSSEARCHESREQUEST._serialized_start=17102
-  _POSTMODELSSEARCHESREQUEST._serialized_end=17271
-  _SINGLEMODELRESPONSE._serialized_start=17273
-  _SINGLEMODELRESPONSE._serialized_end=17375
-  _MULTIMODELRESPONSE._serialized_start=17377
-  _MULTIMODELRESPONSE._serialized_end=17485
-  _PATCHMODELVERSIONSREQUEST._serialized_start=17488
-  _PATCHMODELVERSIONSREQUEST._serialized_end=17650
-  _GETMODELVERSIONREQUEST._serialized_start=17652
-  _GETMODELVERSIONREQUEST._serialized_end=17763
-  _LISTMODELVERSIONSREQUEST._serialized_start=17766
-  _LISTMODELVERSIONSREQUEST._serialized_end=18091
-  _DELETEMODELVERSIONREQUEST._serialized_start=18093
-  _DELETEMODELVERSIONREQUEST._serialized_end=18207
-  _SINGLEMODELVERSIONRESPONSE._serialized_start=18209
-  _SINGLEMODELVERSIONRESPONSE._serialized_end=18333
-  _MULTIMODELVERSIONRESPONSE._serialized_start=18336
-  _MULTIMODELVERSIONRESPONSE._serialized_end=18466
-  _POSTMODELVERSIONSREQUEST._serialized_start=18469
-  _POSTMODELVERSIONSREQUEST._serialized_end=18708
-  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_start=18711
-  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_end=18888
-  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_start=18891
-  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_end=19064
-  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_start=19066
-  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_end=19117
-  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_start=19119
-  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_end=19172
-  _MODELVERSIONPUBLISHREQUEST._serialized_start=19174
-  _MODELVERSIONPUBLISHREQUEST._serialized_end=19222
-  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_start=19225
-  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_end=19389
-  _MODELVERSIONUNPUBLISHREQUEST._serialized_start=19391
-  _MODELVERSIONUNPUBLISHREQUEST._serialized_end=19441
-  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_start=19444
-  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_end=19612
-  _POSTEVALUATIONSREQUEST._serialized_start=19614
-  _POSTEVALUATIONSREQUEST._serialized_end=19736
-  _LISTEVALUATIONSREQUEST._serialized_start=19738
-  _LISTEVALUATIONSREQUEST._serialized_end=19843
-  _GETEVALUATIONREQUEST._serialized_start=19846
-  _GETEVALUATIONREQUEST._serialized_end=19983
-  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_start=19986
-  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_end=20164
-  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_start=20167
-  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_end=20328
-  _GETMODELVERSIONEVALUATIONREQUEST._serialized_start=20331
-  _GETMODELVERSIONEVALUATIONREQUEST._serialized_end=20524
-  _SINGLEEVALMETRICSRESPONSE._serialized_start=20526
-  _SINGLEEVALMETRICSRESPONSE._serialized_end=20647
-  _MULTIEVALMETRICSRESPONSE._serialized_start=20649
-  _MULTIEVALMETRICSRESPONSE._serialized_end=20769
-  _POSTMODELVERSIONMETRICSREQUEST._serialized_start=20772
-  _POSTMODELVERSIONMETRICSREQUEST._serialized_end=20983
-  _GETMODELVERSIONMETRICSREQUEST._serialized_start=20986
-  _GETMODELVERSIONMETRICSREQUEST._serialized_end=21147
-  _GETMODELTYPEREQUEST._serialized_start=21149
-  _GETMODELTYPEREQUEST._serialized_end=21242
-  _LISTMODELTYPESREQUEST._serialized_start=21244
-  _LISTMODELTYPESREQUEST._serialized_end=21348
-  _LISTOPENSOURCELICENSESREQUEST._serialized_start=21350
-  _LISTOPENSOURCELICENSESREQUEST._serialized_end=21381
-  _LISTOPENSOURCELICENSESRESPONSE._serialized_start=21383
-  _LISTOPENSOURCELICENSESRESPONSE._serialized_end=21478
-  _SINGLEMODELTYPERESPONSE._serialized_start=21480
-  _SINGLEMODELTYPERESPONSE._serialized_end=21601
-  _MULTIMODELTYPERESPONSE._serialized_start=21604
-  _MULTIMODELTYPERESPONSE._serialized_end=21846
-  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_start=21849
-  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_end=21998
-  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_start=22001
-  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_end=22164
-  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=22167
-  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=22329
-  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=22332
-  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=22494
-  _LISTMODELREFERENCESREQUEST._serialized_start=22496
-  _LISTMODELREFERENCESREQUEST._serialized_end=22623
-  _MULTIMODELREFERENCERESPONSE._serialized_start=22626
-  _MULTIMODELREFERENCERESPONSE._serialized_end=22756
-  _MULTIOUTPUTRESPONSE._serialized_start=22758
-  _MULTIOUTPUTRESPONSE._serialized_end=22869
-  _LISTSCOPESREQUEST._serialized_start=22871
-  _LISTSCOPESREQUEST._serialized_end=22957
-  _MYSCOPESREQUEST._serialized_start=22959
-  _MYSCOPESREQUEST._serialized_end=23025
-  _MYSCOPESUSERREQUEST._serialized_start=23027
-  _MYSCOPESUSERREQUEST._serialized_end=23097
-  _MYSCOPESROOTREQUEST._serialized_start=23099
-  _MYSCOPESROOTREQUEST._serialized_end=23120
-  _MULTISCOPEDEPSRESPONSE._serialized_start=23123
-  _MULTISCOPEDEPSRESPONSE._serialized_end=23288
-  _MULTISCOPERESPONSE._serialized_start=23291
-  _MULTISCOPERESPONSE._serialized_end=23451
-  _MULTISCOPEUSERRESPONSE._serialized_start=23454
-  _MULTISCOPEUSERRESPONSE._serialized_end=23586
-  _MULTISCOPEROOTRESPONSE._serialized_start=23589
-  _MULTISCOPEROOTRESPONSE._serialized_end=23721
-  _GETSEARCHREQUEST._serialized_start=23723
-  _GETSEARCHREQUEST._serialized_end=23802
-  _LISTSEARCHESREQUEST._serialized_start=23804
-  _LISTSEARCHESREQUEST._serialized_end=23906
-  _POSTSEARCHESREQUEST._serialized_start=23909
-  _POSTSEARCHESREQUEST._serialized_end=24105
-  _PATCHINPUTSSEARCHESREQUEST._serialized_start=24108
-  _PATCHINPUTSSEARCHESREQUEST._serialized_end=24241
-  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_start=24244
-  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_end=24382
-  _PATCHSEARCHESREQUEST._serialized_start=24384
-  _PATCHSEARCHESREQUEST._serialized_end=24511
-  _POSTSEARCHESBYIDREQUEST._serialized_start=24514
-  _POSTSEARCHESBYIDREQUEST._serialized_end=24646
-  _DELETESEARCHREQUEST._serialized_start=24648
-  _DELETESEARCHREQUEST._serialized_end=24730
-  _POSTANNOTATIONSSEARCHESREQUEST._serialized_start=24733
-  _POSTANNOTATIONSSEARCHESREQUEST._serialized_end=24900
-  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_start=24902
-  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25001
-  _POSTINPUTSSEARCHESREQUEST._serialized_start=25004
-  _POSTINPUTSSEARCHESREQUEST._serialized_end=25186
-  _SINGLESEARCHRESPONSE._serialized_start=25188
-  _SINGLESEARCHRESPONSE._serialized_end=25293
-  _MULTISEARCHRESPONSE._serialized_start=25296
-  _MULTISEARCHRESPONSE._serialized_end=25533
-  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25536
-  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25812
-  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25814
-  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25910
-  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25912
-  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25997
-  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_start=26000
-  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_end=26157
-  _LISTANNOTATIONFILTERSREQUEST._serialized_start=26159
-  _LISTANNOTATIONFILTERSREQUEST._serialized_end=26270
-  _GETANNOTATIONFILTERREQUEST._serialized_start=26272
-  _GETANNOTATIONFILTERREQUEST._serialized_end=26379
-  _POSTANNOTATIONFILTERSREQUEST._serialized_start=26382
-  _POSTANNOTATIONFILTERSREQUEST._serialized_end=26521
-  _PATCHANNOTATIONFILTERSREQUEST._serialized_start=26524
-  _PATCHANNOTATIONFILTERSREQUEST._serialized_end=26680
-  _DELETEANNOTATIONFILTERSREQUEST._serialized_start=26682
-  _DELETEANNOTATIONFILTERSREQUEST._serialized_end=26794
-  _MULTIANNOTATIONFILTERRESPONSE._serialized_start=26797
-  _MULTIANNOTATIONFILTERRESPONSE._serialized_end=26939
-  _SINGLEANNOTATIONFILTERRESPONSE._serialized_start=26942
-  _SINGLEANNOTATIONFILTERRESPONSE._serialized_end=27078
-  _GETUSERREQUEST._serialized_start=27080
-  _GETUSERREQUEST._serialized_end=27172
-  _SINGLEUSERRESPONSE._serialized_start=27174
-  _SINGLEUSERRESPONSE._serialized_end=27273
-  _POSTVALIDATEPASSWORDREQUEST._serialized_start=27275
-  _POSTVALIDATEPASSWORDREQUEST._serialized_end=27395
-  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_start=27398
-  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_end=27540
-  _GETWORKFLOWREQUEST._serialized_start=27543
-  _GETWORKFLOWREQUEST._serialized_end=27730
-  _LISTWORKFLOWSREQUEST._serialized_start=27733
-  _LISTWORKFLOWSREQUEST._serialized_end=28048
-  _POSTWORKFLOWSREQUEST._serialized_start=28050
-  _POSTWORKFLOWSREQUEST._serialized_end=28164
-  _PATCHWORKFLOWSREQUEST._serialized_start=28167
-  _PATCHWORKFLOWSREQUEST._serialized_end=28298
-  _PATCHWORKFLOWIDSREQUEST._serialized_start=28301
-  _PATCHWORKFLOWIDSREQUEST._serialized_end=28434
-  _DELETEWORKFLOWREQUEST._serialized_start=28436
-  _DELETEWORKFLOWREQUEST._serialized_end=28529
-  _DELETEWORKFLOWSREQUEST._serialized_start=28531
-  _DELETEWORKFLOWSREQUEST._serialized_end=28637
-  _SINGLEWORKFLOWRESPONSE._serialized_start=28639
-  _SINGLEWORKFLOWRESPONSE._serialized_end=28750
-  _MULTIWORKFLOWRESPONSE._serialized_start=28752
-  _MULTIWORKFLOWRESPONSE._serialized_end=28869
-  _POSTWORKFLOWRESULTSREQUEST._serialized_start=28872
-  _POSTWORKFLOWRESULTSREQUEST._serialized_end=29165
-  _POSTWORKFLOWRESULTSRESPONSE._serialized_start=29168
-  _POSTWORKFLOWRESULTSRESPONSE._serialized_end=29384
-  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_start=29387
-  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_end=29660
-  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_start=29663
-  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_end=29805
-  _LISTWORKFLOWVERSIONSREQUEST._serialized_start=29808
-  _LISTWORKFLOWVERSIONSREQUEST._serialized_end=29939
-  _GETWORKFLOWVERSIONREQUEST._serialized_start=29941
-  _GETWORKFLOWVERSIONREQUEST._serialized_end=30067
-  _DELETEWORKFLOWVERSIONSREQUEST._serialized_start=30070
-  _DELETEWORKFLOWVERSIONSREQUEST._serialized_end=30201
-  _PATCHWORKFLOWVERSIONSREQUEST._serialized_start=30204
-  _PATCHWORKFLOWVERSIONSREQUEST._serialized_end=30378
-  _MULTIWORKFLOWVERSIONRESPONSE._serialized_start=30381
-  _MULTIWORKFLOWVERSIONRESPONSE._serialized_end=30520
-  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_start=30523
-  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_end=30656
-  _POSTAPPDUPLICATIONSREQUEST._serialized_start=30659
-  _POSTAPPDUPLICATIONSREQUEST._serialized_end=30792
-  _GETAPPDUPLICATIONREQUEST._serialized_start=30794
-  _GETAPPDUPLICATIONREQUEST._serialized_end=30897
-  _LISTAPPDUPLICATIONSREQUEST._serialized_start=30899
-  _LISTAPPDUPLICATIONSREQUEST._serialized_end=31008
-  _MULTIAPPDUPLICATIONSRESPONSE._serialized_start=31011
-  _MULTIAPPDUPLICATIONSRESPONSE._serialized_end=31142
-  _SINGLEAPPDUPLICATIONRESPONSE._serialized_start=31145
-  _SINGLEAPPDUPLICATIONRESPONSE._serialized_end=31275
-  _POSTTASKSREQUEST._serialized_start=31277
-  _POSTTASKSREQUEST._serialized_end=31379
-  _GETTASKREQUEST._serialized_start=31381
-  _GETTASKREQUEST._serialized_end=31490
-  _LISTTASKSREQUEST._serialized_start=31493
-  _LISTTASKSREQUEST._serialized_end=31731
-  _PATCHTASKSREQUEST._serialized_start=31733
-  _PATCHTASKSREQUEST._serialized_end=31852
-  _DELETETASKSREQUEST._serialized_start=31854
-  _DELETETASKSREQUEST._serialized_end=31936
-  _MULTITASKRESPONSE._serialized_start=31938
-  _MULTITASKRESPONSE._serialized_end=32043
-  _SINGLETASKRESPONSE._serialized_start=32045
-  _SINGLETASKRESPONSE._serialized_end=32144
-  _GETTASKCOUNTREQUEST._serialized_start=32146
-  _GETTASKCOUNTREQUEST._serialized_end=32251
-  _SINGLETASKCOUNTRESPONSE._serialized_start=32254
-  _SINGLETASKCOUNTRESPONSE._serialized_end=32411
-  _POSTLABELORDERSREQUEST._serialized_start=32413
-  _POSTLABELORDERSREQUEST._serialized_end=32534
-  _GETLABELORDERREQUEST._serialized_start=32536
-  _GETLABELORDERREQUEST._serialized_end=32631
-  _LISTLABELORDERSREQUEST._serialized_start=32633
-  _LISTLABELORDERSREQUEST._serialized_end=32738
-  _PATCHLABELORDERSREQUEST._serialized_start=32741
-  _PATCHLABELORDERSREQUEST._serialized_end=32879
-  _DELETELABELORDERSREQUEST._serialized_start=32881
-  _DELETELABELORDERSREQUEST._serialized_end=32969
-  _MULTILABELORDERRESPONSE._serialized_start=32971
-  _MULTILABELORDERRESPONSE._serialized_end=33095
-  _SINGLELABELORDERRESPONSE._serialized_start=33097
-  _SINGLELABELORDERRESPONSE._serialized_end=33215
-  _POSTCOLLECTORSREQUEST._serialized_start=33217
-  _POSTCOLLECTORSREQUEST._serialized_end=33334
-  _PATCHCOLLECTORSREQUEST._serialized_start=33337
-  _PATCHCOLLECTORSREQUEST._serialized_end=33471
-  _DELETECOLLECTORSREQUEST._serialized_start=33473
-  _DELETECOLLECTORSREQUEST._serialized_end=33580
-  _GETCOLLECTORREQUEST._serialized_start=33582
-  _GETCOLLECTORREQUEST._serialized_end=33674
-  _LISTCOLLECTORSREQUEST._serialized_start=33676
-  _LISTCOLLECTORSREQUEST._serialized_end=33780
-  _MULTICOLLECTORRESPONSE._serialized_start=33782
-  _MULTICOLLECTORRESPONSE._serialized_end=33896
-  _SINGLECOLLECTORRESPONSE._serialized_start=33898
-  _SINGLECOLLECTORRESPONSE._serialized_end=34012
-  _POSTSTATVALUESREQUEST._serialized_start=34014
-  _POSTSTATVALUESREQUEST._serialized_end=34132
-  _MULTISTATVALUERESPONSE._serialized_start=34134
-  _MULTISTATVALUERESPONSE._serialized_end=34255
-  _POSTSTATVALUESAGGREGATEREQUEST._serialized_start=34258
-  _POSTSTATVALUESAGGREGATEREQUEST._serialized_end=34416
-  _MULTISTATVALUEAGGREGATERESPONSE._serialized_start=34419
-  _MULTISTATVALUEAGGREGATERESPONSE._serialized_end=34575
-  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_start=34577
-  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_end=34696
-  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_start=34699
-  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_end=34832
-  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_start=34834
-  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_end=34960
-  _GETMODULEREQUEST._serialized_start=34962
-  _GETMODULEREQUEST._serialized_end=35075
-  _LISTMODULESREQUEST._serialized_start=35078
-  _LISTMODULESREQUEST._serialized_end=35228
-  _POSTMODULESREQUEST._serialized_start=35230
-  _POSTMODULESREQUEST._serialized_end=35338
-  _PATCHMODULESREQUEST._serialized_start=35340
-  _PATCHMODULESREQUEST._serialized_end=35465
-  _DELETEMODULESREQUEST._serialized_start=35467
-  _DELETEMODULESREQUEST._serialized_end=35551
-  _SINGLEMODULERESPONSE._serialized_start=35553
-  _SINGLEMODULERESPONSE._serialized_end=35658
-  _MULTIMODULERESPONSE._serialized_start=35660
-  _MULTIMODULERESPONSE._serialized_end=35771
-  _GETMODULEVERSIONREQUEST._serialized_start=35773
-  _GETMODULEVERSIONREQUEST._serialized_end=35893
-  _LISTMODULEVERSIONSREQUEST._serialized_start=35895
-  _LISTMODULEVERSIONSREQUEST._serialized_end=36022
-  _POSTMODULEVERSIONSREQUEST._serialized_start=36025
-  _POSTMODULEVERSIONSREQUEST._serialized_end=36174
-  _DELETEMODULEVERSIONSREQUEST._serialized_start=36176
-  _DELETEMODULEVERSIONSREQUEST._serialized_end=36286
-  _SINGLEMODULEVERSIONRESPONSE._serialized_start=36288
-  _SINGLEMODULEVERSIONRESPONSE._serialized_end=36415
-  _MULTIMODULEVERSIONRESPONSE._serialized_start=36418
-  _MULTIMODULEVERSIONRESPONSE._serialized_end=36551
-  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_start=36553
-  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_end=36673
-  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36675
-  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36792
-  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=36795
-  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=36953
-  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_start=36955
-  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_end=37080
-  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_start=37082
-  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_end=37182
-  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_start=37185
-  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_end=37340
-  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_start=37343
-  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_end=37504
-  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_start=37506
-  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_end=37604
-  _POSTBULKOPERATIONSREQUEST._serialized_start=37607
-  _POSTBULKOPERATIONSREQUEST._serialized_end=37737
-  _LISTBULKOPERATIONSREQUEST._serialized_start=37739
-  _LISTBULKOPERATIONSREQUEST._serialized_end=37847
-  _GETBULKOPERATIONREQUEST._serialized_start=37849
-  _GETBULKOPERATIONREQUEST._serialized_end=37935
-  _CANCELBULKOPERATIONREQUEST._serialized_start=37937
-  _CANCELBULKOPERATIONREQUEST._serialized_end=38027
-  _DELETEBULKOPERATIONREQUEST._serialized_start=38029
-  _DELETEBULKOPERATIONREQUEST._serialized_end=38119
-  _SINGLEBULKOPERATIONSRESPONSE._serialized_start=38122
-  _SINGLEBULKOPERATIONSRESPONSE._serialized_end=38250
-  _MULTIBULKOPERATIONSRESPONSE._serialized_start=38252
-  _MULTIBULKOPERATIONSRESPONSE._serialized_end=38379
-  _PUTTASKASSIGNMENTSREQUEST._serialized_start=38381
-  _PUTTASKASSIGNMENTSREQUEST._serialized_end=38492
-  _LISTINPUTSADDJOBSREQUEST._serialized_start=38494
-  _LISTINPUTSADDJOBSREQUEST._serialized_end=38601
-  _GETINPUTSADDJOBREQUEST._serialized_start=38603
-  _GETINPUTSADDJOBREQUEST._serialized_end=38688
-  _CANCELINPUTSADDJOBREQUEST._serialized_start=38690
-  _CANCELINPUTSADDJOBREQUEST._serialized_end=38778
-  _MULTIINPUTSADDJOBRESPONSE._serialized_start=38781
-  _MULTIINPUTSADDJOBRESPONSE._serialized_end=38912
-  _SINGLEINPUTSADDJOBRESPONSE._serialized_start=38914
-  _SINGLEINPUTSADDJOBRESPONSE._serialized_end=39039
-  _POSTUPLOADSREQUEST._serialized_start=39041
-  _POSTUPLOADSREQUEST._serialized_end=39149
-  _DELETEUPLOADSREQUEST._serialized_start=39151
-  _DELETEUPLOADSREQUEST._serialized_end=39235
-  _LISTUPLOADSREQUEST._serialized_start=39237
-  _LISTUPLOADSREQUEST._serialized_end=39338
-  _GETUPLOADREQUEST._serialized_start=39340
-  _GETUPLOADREQUEST._serialized_end=39426
-  _SINGLEUPLOADRESPONSE._serialized_start=39428
-  _SINGLEUPLOADRESPONSE._serialized_end=39533
-  _MULTIUPLOADRESPONSE._serialized_start=39535
-  _MULTIUPLOADRESPONSE._serialized_end=39640
-  _PUTUPLOADCONTENTPARTSREQUEST._serialized_start=39643
-  _PUTUPLOADCONTENTPARTSREQUEST._serialized_end=39797
-  _POSTINPUTSDATASOURCESREQUEST._serialized_start=39800
-  _POSTINPUTSDATASOURCESREQUEST._serialized_end=39973
-  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_start=39975
-  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_end=40089
-  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_start=40091
-  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_end=40205
-  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_start=40208
-  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_end=40354
-  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_start=40357
-  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_end=40503
-  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_start=40505
-  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_end=40602
-  _POSTINPUTSUPLOADSREQUEST._serialized_start=40604
-  _POSTINPUTSUPLOADSREQUEST._serialized_end=40731
-  _V2._serialized_start=40849
-  _V2._serialized_end=90395
+  _LISTAPPSREQUEST._serialized_end=2411
+  _POSTAPPSREQUEST._serialized_start=2413
+  _POSTAPPSREQUEST._serialized_end=2512
+  _DELETEAPPREQUEST._serialized_start=2514
+  _DELETEAPPREQUEST._serialized_end=2581
+  _PATCHAPPSREQUEST._serialized_start=2584
+  _PATCHAPPSREQUEST._serialized_end=2769
+  _PATCHAPPREQUEST._serialized_start=2772
+  _PATCHAPPREQUEST._serialized_end=2955
+  _PATCHAPPSIDSREQUEST._serialized_start=2958
+  _PATCHAPPSIDSREQUEST._serialized_end=3087
+  _POSTAPPSSEARCHESREQUEST._serialized_start=3090
+  _POSTAPPSSEARCHESREQUEST._serialized_end=3253
+  _SINGLEAPPRESPONSE._serialized_start=3255
+  _SINGLEAPPRESPONSE._serialized_end=3351
+  _MULTIAPPRESPONSE._serialized_start=3353
+  _MULTIAPPRESPONSE._serialized_end=3455
+  _LISTCOLLABORATORSREQUEST._serialized_start=3458
+  _LISTCOLLABORATORSREQUEST._serialized_end=3597
+  _POSTCOLLABORATORSREQUEST._serialized_start=3599
+  _POSTCOLLABORATORSREQUEST._serialized_end=3725
+  _PATCHCOLLABORATORSREQUEST._serialized_start=3728
+  _PATCHCOLLABORATORSREQUEST._serialized_end=3871
+  _DELETECOLLABORATORSREQUEST._serialized_start=3873
+  _DELETECOLLABORATORSREQUEST._serialized_end=3997
+  _MULTICOLLABORATORSRESPONSE._serialized_start=4000
+  _MULTICOLLABORATORSRESPONSE._serialized_end=4130
+  _LISTCOLLABORATIONSREQUEST._serialized_start=4132
+  _LISTCOLLABORATIONSREQUEST._serialized_end=4240
+  _MULTICOLLABORATIONSRESPONSE._serialized_start=4243
+  _MULTICOLLABORATIONSRESPONSE._serialized_end=4376
+  _GETSTATUSCODEREQUEST._serialized_start=4378
+  _GETSTATUSCODEREQUEST._serialized_end=4424
+  _LISTSTATUSCODESREQUEST._serialized_start=4426
+  _LISTSTATUSCODESREQUEST._serialized_end=4450
+  _SINGLESTATUSCODERESPONSE._serialized_start=4452
+  _SINGLESTATUSCODERESPONSE._serialized_end=4523
+  _MULTISTATUSCODERESPONSE._serialized_start=4525
+  _MULTISTATUSCODERESPONSE._serialized_end=4642
+  _GETCONCEPTREQUEST._serialized_start=4644
+  _GETCONCEPTREQUEST._serialized_end=4732
+  _LISTCONCEPTSREQUEST._serialized_start=4734
+  _LISTCONCEPTSREQUEST._serialized_end=4836
+  _LISTMODELCONCEPTSREQUEST._serialized_start=4839
+  _LISTMODELCONCEPTSREQUEST._serialized_end=4984
+  _POSTCONCEPTSSEARCHESREQUEST._serialized_start=4987
+  _POSTCONCEPTSSEARCHESREQUEST._serialized_end=5162
+  _POSTCONCEPTSREQUEST._serialized_start=5164
+  _POSTCONCEPTSREQUEST._serialized_end=5275
+  _PATCHCONCEPTSREQUEST._serialized_start=5278
+  _PATCHCONCEPTSREQUEST._serialized_end=5406
+  _GETCONCEPTCOUNTSREQUEST._serialized_start=5408
+  _GETCONCEPTCOUNTSREQUEST._serialized_end=5514
+  _SINGLECONCEPTRESPONSE._serialized_start=5516
+  _SINGLECONCEPTRESPONSE._serialized_end=5624
+  _MULTICONCEPTRESPONSE._serialized_start=5626
+  _MULTICONCEPTRESPONSE._serialized_end=5740
+  _MULTICONCEPTCOUNTRESPONSE._serialized_start=5743
+  _MULTICONCEPTCOUNTRESPONSE._serialized_end=5873
+  _LISTCONCEPTRELATIONSREQUEST._serialized_start=5876
+  _LISTCONCEPTRELATIONSREQUEST._serialized_end=6053
+  _POSTCONCEPTRELATIONSREQUEST._serialized_start=6056
+  _POSTCONCEPTRELATIONSREQUEST._serialized_end=6212
+  _DELETECONCEPTRELATIONSREQUEST._serialized_start=6214
+  _DELETECONCEPTRELATIONSREQUEST._serialized_end=6327
+  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_start=6329
+  _LISTKNOWLEDGEGRAPHSREQUEST._serialized_end=6406
+  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_start=6409
+  _POSTKNOWLEDGEGRAPHSREQUEST._serialized_end=6542
+  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_start=6545
+  _POSTCONCEPTMAPPINGJOBSREQUEST._serialized_end=6688
+  _MULTICONCEPTRELATIONRESPONSE._serialized_start=6691
+  _MULTICONCEPTRELATIONRESPONSE._serialized_end=6830
+  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_start=6833
+  _MULTIKNOWLEDGEGRAPHRESPONSE._serialized_end=6969
+  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_start=6971
+  _MULTICONCEPTMAPPINGJOBRESPONSE._serialized_end=7061
+  _GETCONCEPTLANGUAGEREQUEST._serialized_start=7063
+  _GETCONCEPTLANGUAGEREQUEST._serialized_end=7177
+  _LISTCONCEPTLANGUAGESREQUEST._serialized_start=7180
+  _LISTCONCEPTLANGUAGESREQUEST._serialized_end=7310
+  _PATCHCONCEPTLANGUAGESREQUEST._serialized_start=7313
+  _PATCHCONCEPTLANGUAGESREQUEST._serialized_end=7486
+  _POSTCONCEPTLANGUAGESREQUEST._serialized_start=7489
+  _POSTCONCEPTLANGUAGESREQUEST._serialized_end=7645
+  _SINGLECONCEPTLANGUAGERESPONSE._serialized_start=7648
+  _SINGLECONCEPTLANGUAGERESPONSE._serialized_end=7781
+  _MULTICONCEPTLANGUAGERESPONSE._serialized_start=7784
+  _MULTICONCEPTLANGUAGERESPONSE._serialized_end=7923
+  _GETINPUTREQUEST._serialized_start=7925
+  _GETINPUTREQUEST._serialized_end=8009
+  _GETVIDEOMANIFESTREQUEST._serialized_start=8011
+  _GETVIDEOMANIFESTREQUEST._serialized_end=8103
+  _GETINPUTSAMPLESREQUEST._serialized_start=8105
+  _GETINPUTSAMPLESREQUEST._serialized_end=8213
+  _LISTINPUTSREQUEST._serialized_start=8216
+  _LISTINPUTSREQUEST._serialized_end=8374
+  _STREAMINPUTSREQUEST._serialized_start=8377
+  _STREAMINPUTSREQUEST._serialized_end=8523
+  _POSTINPUTSREQUEST._serialized_start=8526
+  _POSTINPUTSREQUEST._serialized_end=8737
+  _PATCHINPUTSREQUEST._serialized_start=8739
+  _PATCHINPUTSREQUEST._serialized_end=8861
+  _DELETEINPUTREQUEST._serialized_start=8863
+  _DELETEINPUTREQUEST._serialized_end=8950
+  _DELETEINPUTSREQUEST._serialized_start=8952
+  _DELETEINPUTSREQUEST._serialized_end=9041
+  _SINGLEINPUTRESPONSE._serialized_start=9043
+  _SINGLEINPUTRESPONSE._serialized_end=9145
+  _GETVIDEOMANIFESTRESPONSE._serialized_start=9147
+  _GETVIDEOMANIFESTRESPONSE._serialized_end=9240
+  _MULTIINPUTRESPONSE._serialized_start=9243
+  _MULTIINPUTRESPONSE._serialized_end=9403
+  _MULTIINPUTANNOTATIONRESPONSE._serialized_start=9405
+  _MULTIINPUTANNOTATIONRESPONSE._serialized_end=9519
+  _SINGLEINPUTCOUNTRESPONSE._serialized_start=9521
+  _SINGLEINPUTCOUNTRESPONSE._serialized_end=9634
+  _GETINPUTCOUNTREQUEST._serialized_start=9636
+  _GETINPUTCOUNTREQUEST._serialized_end=9707
+  _LISTDATASETSREQUEST._serialized_start=9710
+  _LISTDATASETSREQUEST._serialized_end=10005
+  _GETDATASETREQUEST._serialized_start=10007
+  _GETDATASETREQUEST._serialized_end=10122
+  _POSTDATASETSREQUEST._serialized_start=10124
+  _POSTDATASETSREQUEST._serialized_end=10235
+  _PATCHDATASETSREQUEST._serialized_start=10238
+  _PATCHDATASETSREQUEST._serialized_end=10366
+  _DELETEDATASETSREQUEST._serialized_start=10368
+  _DELETEDATASETSREQUEST._serialized_end=10461
+  _MULTIDATASETRESPONSE._serialized_start=10463
+  _MULTIDATASETRESPONSE._serialized_end=10577
+  _SINGLEDATASETRESPONSE._serialized_start=10579
+  _SINGLEDATASETRESPONSE._serialized_end=10687
+  _LISTDATASETINPUTSREQUEST._serialized_start=10689
+  _LISTDATASETINPUTSREQUEST._serialized_end=10816
+  _GETDATASETINPUTREQUEST._serialized_start=10818
+  _GETDATASETINPUTREQUEST._serialized_end=10929
+  _POSTDATASETINPUTSREQUEST._serialized_start=10932
+  _POSTDATASETINPUTSREQUEST._serialized_end=11117
+  _DELETEDATASETINPUTSREQUEST._serialized_start=11119
+  _DELETEDATASETINPUTSREQUEST._serialized_end=11235
+  _MULTIDATASETINPUTRESPONSE._serialized_start=11238
+  _MULTIDATASETINPUTRESPONSE._serialized_end=11448
+  _SINGLEDATASETINPUTRESPONSE._serialized_start=11450
+  _SINGLEDATASETINPUTRESPONSE._serialized_end=11574
+  _LISTDATASETVERSIONSREQUEST._serialized_start=11577
+  _LISTDATASETVERSIONSREQUEST._serialized_end=11706
+  _GETDATASETVERSIONREQUEST._serialized_start=11708
+  _GETDATASETVERSIONREQUEST._serialized_end=11831
+  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_start=11834
+  _LISTDATASETVERSIONMETRICSGROUPSREQUEST._serialized_end=12126
+  _POSTDATASETVERSIONSREQUEST._serialized_start=12129
+  _POSTDATASETVERSIONSREQUEST._serialized_end=12282
+  _PATCHDATASETVERSIONSREQUEST._serialized_start=12285
+  _PATCHDATASETVERSIONSREQUEST._serialized_end=12455
+  _DELETEDATASETVERSIONSREQUEST._serialized_start=12458
+  _DELETEDATASETVERSIONSREQUEST._serialized_end=12586
+  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_start=12589
+  _PUTDATASETVERSIONEXPORTSREQUEST._serialized_end=12772
+  _MULTIDATASETVERSIONRESPONSE._serialized_start=12775
+  _MULTIDATASETVERSIONRESPONSE._serialized_end=12911
+  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_start=12914
+  _MULTIDATASETVERSIONEXPORTRESPONSE._serialized_end=13053
+  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_start=13056
+  _MULTIDATASETVERSIONMETRICSGROUPRESPONSE._serialized_end=13230
+  _SINGLEDATASETVERSIONRESPONSE._serialized_start=13233
+  _SINGLEDATASETVERSIONRESPONSE._serialized_end=13363
+  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_start=13365
+  _GETDATASETINPUTSSEARCHADDJOBREQUEST._serialized_end=13467
+  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_start=13470
+  _SINGLEDATASETINPUTSSEARCHADDJOBRESPONSE._serialized_end=13610
+  _POSTMODELOUTPUTSREQUEST._serialized_start=13613
+  _POSTMODELOUTPUTSREQUEST._serialized_end=13798
+  _LISTMODELINPUTSREQUEST._serialized_start=13801
+  _LISTMODELINPUTSREQUEST._serialized_end=13944
+  _GETKEYREQUEST._serialized_start=13946
+  _GETKEYREQUEST._serialized_end=14026
+  _LISTKEYSREQUEST._serialized_start=14029
+  _LISTKEYSREQUEST._serialized_end=14183
+  _LISTAPPKEYSREQUEST._serialized_start=14185
+  _LISTAPPKEYSREQUEST._serialized_end=14286
+  _POSTKEYSREQUEST._serialized_start=14288
+  _POSTKEYSREQUEST._serialized_end=14387
+  _DELETEKEYREQUEST._serialized_start=14389
+  _DELETEKEYREQUEST._serialized_end=14472
+  _PATCHKEYSREQUEST._serialized_start=14474
+  _PATCHKEYSREQUEST._serialized_end=14590
+  _SINGLEKEYRESPONSE._serialized_start=14592
+  _SINGLEKEYRESPONSE._serialized_end=14688
+  _MULTIKEYRESPONSE._serialized_start=14690
+  _MULTIKEYRESPONSE._serialized_end=14792
+  _GETMODELREQUEST._serialized_start=14795
+  _GETMODELREQUEST._serialized_end=14968
+  _LISTMODELSREQUEST._serialized_start=14971
+  _LISTMODELSREQUEST._serialized_end=15596
+  _GETRESOURCECOUNTSREQUEST._serialized_start=15598
+  _GETRESOURCECOUNTSREQUEST._serialized_end=15673
+  _GETRESOURCECOUNTSRESPONSE._serialized_start=15676
+  _GETRESOURCECOUNTSRESPONSE._serialized_end=15818
+  _PATCHMODELTOOLKITSREQUEST._serialized_start=15821
+  _PATCHMODELTOOLKITSREQUEST._serialized_end=15949
+  _PATCHMODELCHECKCONSENTSREQUEST._serialized_start=15952
+  _PATCHMODELCHECKCONSENTSREQUEST._serialized_end=16091
+  _PATCHMODELUSECASESREQUEST._serialized_start=16094
+  _PATCHMODELUSECASESREQUEST._serialized_end=16222
+  _PATCHMODELLANGUAGESREQUEST._serialized_start=16225
+  _PATCHMODELLANGUAGESREQUEST._serialized_end=16355
+  _MULTIMODELTOOLKITRESPONSE._serialized_start=16357
+  _MULTIMODELTOOLKITRESPONSE._serialized_end=16447
+  _MULTIMODELCHECKCONSENTRESPONSE._serialized_start=16449
+  _MULTIMODELCHECKCONSENTRESPONSE._serialized_end=16550
+  _MULTIMODELUSECASERESPONSE._serialized_start=16552
+  _MULTIMODELUSECASERESPONSE._serialized_end=16642
+  _MULTIMODELLANGUAGERESPONSE._serialized_start=16644
+  _MULTIMODELLANGUAGERESPONSE._serialized_end=16736
+  _POSTMODELSREQUEST._serialized_start=16739
+  _POSTMODELSREQUEST._serialized_end=16884
+  _PATCHMODELSREQUEST._serialized_start=16886
+  _PATCHMODELSREQUEST._serialized_end=17008
+  _IDUPDATESOURCE._serialized_start=17010
+  _IDUPDATESOURCE._serialized_end=17054
+  _PATCHMODELIDSREQUEST._serialized_start=17057
+  _PATCHMODELIDSREQUEST._serialized_end=17187
+  _DELETEMODELREQUEST._serialized_start=17189
+  _DELETEMODELREQUEST._serialized_end=17276
+  _DELETEMODELSREQUEST._serialized_start=17278
+  _DELETEMODELSREQUEST._serialized_end=17381
+  _POSTMODELSSEARCHESREQUEST._serialized_start=17384
+  _POSTMODELSSEARCHESREQUEST._serialized_end=17553
+  _SINGLEMODELRESPONSE._serialized_start=17555
+  _SINGLEMODELRESPONSE._serialized_end=17657
+  _MULTIMODELRESPONSE._serialized_start=17659
+  _MULTIMODELRESPONSE._serialized_end=17767
+  _PATCHMODELVERSIONSREQUEST._serialized_start=17770
+  _PATCHMODELVERSIONSREQUEST._serialized_end=17932
+  _GETMODELVERSIONREQUEST._serialized_start=17934
+  _GETMODELVERSIONREQUEST._serialized_end=18045
+  _LISTMODELVERSIONSREQUEST._serialized_start=18048
+  _LISTMODELVERSIONSREQUEST._serialized_end=18373
+  _DELETEMODELVERSIONREQUEST._serialized_start=18375
+  _DELETEMODELVERSIONREQUEST._serialized_end=18489
+  _SINGLEMODELVERSIONRESPONSE._serialized_start=18491
+  _SINGLEMODELVERSIONRESPONSE._serialized_end=18615
+  _MULTIMODELVERSIONRESPONSE._serialized_start=18618
+  _MULTIMODELVERSIONRESPONSE._serialized_end=18748
+  _POSTMODELVERSIONSREQUEST._serialized_start=18751
+  _POSTMODELVERSIONSREQUEST._serialized_end=18990
+  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_start=18993
+  _POSTWORKFLOWVERSIONSUNPUBLISHREQUEST._serialized_end=19170
+  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_start=19173
+  _POSTWORKFLOWVERSIONSPUBLISHREQUEST._serialized_end=19346
+  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_start=19348
+  _WORKFLOWVERSIONPUBLISHREQUEST._serialized_end=19399
+  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_start=19401
+  _WORKFLOWVERSIONUNPUBLISHREQUEST._serialized_end=19454
+  _MODELVERSIONPUBLISHREQUEST._serialized_start=19456
+  _MODELVERSIONPUBLISHREQUEST._serialized_end=19504
+  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_start=19507
+  _POSTMODELVERSIONSPUBLISHREQUEST._serialized_end=19671
+  _MODELVERSIONUNPUBLISHREQUEST._serialized_start=19673
+  _MODELVERSIONUNPUBLISHREQUEST._serialized_end=19723
+  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_start=19726
+  _POSTMODELVERSIONSUNPUBLISHREQUEST._serialized_end=19894
+  _POSTEVALUATIONSREQUEST._serialized_start=19896
+  _POSTEVALUATIONSREQUEST._serialized_end=20018
+  _LISTEVALUATIONSREQUEST._serialized_start=20020
+  _LISTEVALUATIONSREQUEST._serialized_end=20125
+  _GETEVALUATIONREQUEST._serialized_start=20128
+  _GETEVALUATIONREQUEST._serialized_end=20265
+  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_start=20268
+  _POSTMODELVERSIONEVALUATIONSREQUEST._serialized_end=20446
+  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_start=20449
+  _LISTMODELVERSIONEVALUATIONSREQUEST._serialized_end=20610
+  _GETMODELVERSIONEVALUATIONREQUEST._serialized_start=20613
+  _GETMODELVERSIONEVALUATIONREQUEST._serialized_end=20806
+  _SINGLEEVALMETRICSRESPONSE._serialized_start=20808
+  _SINGLEEVALMETRICSRESPONSE._serialized_end=20929
+  _MULTIEVALMETRICSRESPONSE._serialized_start=20931
+  _MULTIEVALMETRICSRESPONSE._serialized_end=21051
+  _POSTMODELVERSIONMETRICSREQUEST._serialized_start=21054
+  _POSTMODELVERSIONMETRICSREQUEST._serialized_end=21265
+  _GETMODELVERSIONMETRICSREQUEST._serialized_start=21268
+  _GETMODELVERSIONMETRICSREQUEST._serialized_end=21429
+  _GETMODELTYPEREQUEST._serialized_start=21431
+  _GETMODELTYPEREQUEST._serialized_end=21524
+  _LISTMODELTYPESREQUEST._serialized_start=21526
+  _LISTMODELTYPESREQUEST._serialized_end=21630
+  _LISTOPENSOURCELICENSESREQUEST._serialized_start=21632
+  _LISTOPENSOURCELICENSESREQUEST._serialized_end=21663
+  _LISTOPENSOURCELICENSESRESPONSE._serialized_start=21665
+  _LISTOPENSOURCELICENSESRESPONSE._serialized_end=21760
+  _SINGLEMODELTYPERESPONSE._serialized_start=21762
+  _SINGLEMODELTYPERESPONSE._serialized_end=21883
+  _MULTIMODELTYPERESPONSE._serialized_start=21886
+  _MULTIMODELTYPERESPONSE._serialized_end=22128
+  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_start=22131
+  _GETMODELVERSIONINPUTEXAMPLEREQUEST._serialized_end=22280
+  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_start=22283
+  _LISTMODELVERSIONINPUTEXAMPLESREQUEST._serialized_end=22446
+  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=22449
+  _SINGLEMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=22611
+  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_start=22614
+  _MULTIMODELVERSIONINPUTEXAMPLERESPONSE._serialized_end=22776
+  _LISTMODELREFERENCESREQUEST._serialized_start=22778
+  _LISTMODELREFERENCESREQUEST._serialized_end=22905
+  _MULTIMODELREFERENCERESPONSE._serialized_start=22908
+  _MULTIMODELREFERENCERESPONSE._serialized_end=23038
+  _MULTIOUTPUTRESPONSE._serialized_start=23040
+  _MULTIOUTPUTRESPONSE._serialized_end=23151
+  _LISTSCOPESREQUEST._serialized_start=23153
+  _LISTSCOPESREQUEST._serialized_end=23239
+  _MYSCOPESREQUEST._serialized_start=23241
+  _MYSCOPESREQUEST._serialized_end=23307
+  _MYSCOPESUSERREQUEST._serialized_start=23309
+  _MYSCOPESUSERREQUEST._serialized_end=23379
+  _MYSCOPESROOTREQUEST._serialized_start=23381
+  _MYSCOPESROOTREQUEST._serialized_end=23402
+  _MULTISCOPEDEPSRESPONSE._serialized_start=23405
+  _MULTISCOPEDEPSRESPONSE._serialized_end=23570
+  _MULTISCOPERESPONSE._serialized_start=23573
+  _MULTISCOPERESPONSE._serialized_end=23733
+  _MULTISCOPEUSERRESPONSE._serialized_start=23736
+  _MULTISCOPEUSERRESPONSE._serialized_end=23868
+  _MULTISCOPEROOTRESPONSE._serialized_start=23871
+  _MULTISCOPEROOTRESPONSE._serialized_end=24003
+  _GETSEARCHREQUEST._serialized_start=24005
+  _GETSEARCHREQUEST._serialized_end=24084
+  _LISTSEARCHESREQUEST._serialized_start=24086
+  _LISTSEARCHESREQUEST._serialized_end=24188
+  _POSTSEARCHESREQUEST._serialized_start=24191
+  _POSTSEARCHESREQUEST._serialized_end=24387
+  _PATCHINPUTSSEARCHESREQUEST._serialized_start=24390
+  _PATCHINPUTSSEARCHESREQUEST._serialized_end=24523
+  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_start=24526
+  _PATCHANNOTATIONSSEARCHESREQUEST._serialized_end=24664
+  _PATCHSEARCHESREQUEST._serialized_start=24666
+  _PATCHSEARCHESREQUEST._serialized_end=24793
+  _POSTSEARCHESBYIDREQUEST._serialized_start=24796
+  _POSTSEARCHESBYIDREQUEST._serialized_end=24928
+  _DELETESEARCHREQUEST._serialized_start=24930
+  _DELETESEARCHREQUEST._serialized_end=25012
+  _POSTANNOTATIONSSEARCHESREQUEST._serialized_start=25015
+  _POSTANNOTATIONSSEARCHESREQUEST._serialized_end=25182
+  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25184
+  _DELETEANNOTATIONSEARCHMETRICSREQUEST._serialized_end=25283
+  _POSTINPUTSSEARCHESREQUEST._serialized_start=25286
+  _POSTINPUTSSEARCHESREQUEST._serialized_end=25468
+  _SINGLESEARCHRESPONSE._serialized_start=25470
+  _SINGLESEARCHRESPONSE._serialized_end=25575
+  _MULTISEARCHRESPONSE._serialized_start=25578
+  _MULTISEARCHRESPONSE._serialized_end=25815
+  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=25818
+  _POSTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=26094
+  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_start=26096
+  _GETANNOTATIONSEARCHMETRICSREQUEST._serialized_end=26192
+  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_start=26194
+  _LISTANNOTATIONSEARCHMETRICSREQUEST._serialized_end=26279
+  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_start=26282
+  _MULTIANNOTATIONSEARCHMETRICSRESPONSE._serialized_end=26439
+  _LISTANNOTATIONFILTERSREQUEST._serialized_start=26441
+  _LISTANNOTATIONFILTERSREQUEST._serialized_end=26552
+  _GETANNOTATIONFILTERREQUEST._serialized_start=26554
+  _GETANNOTATIONFILTERREQUEST._serialized_end=26661
+  _POSTANNOTATIONFILTERSREQUEST._serialized_start=26664
+  _POSTANNOTATIONFILTERSREQUEST._serialized_end=26803
+  _PATCHANNOTATIONFILTERSREQUEST._serialized_start=26806
+  _PATCHANNOTATIONFILTERSREQUEST._serialized_end=26962
+  _DELETEANNOTATIONFILTERSREQUEST._serialized_start=26964
+  _DELETEANNOTATIONFILTERSREQUEST._serialized_end=27076
+  _MULTIANNOTATIONFILTERRESPONSE._serialized_start=27079
+  _MULTIANNOTATIONFILTERRESPONSE._serialized_end=27221
+  _SINGLEANNOTATIONFILTERRESPONSE._serialized_start=27224
+  _SINGLEANNOTATIONFILTERRESPONSE._serialized_end=27360
+  _GETUSERREQUEST._serialized_start=27362
+  _GETUSERREQUEST._serialized_end=27454
+  _SINGLEUSERRESPONSE._serialized_start=27456
+  _SINGLEUSERRESPONSE._serialized_end=27555
+  _POSTVALIDATEPASSWORDREQUEST._serialized_start=27557
+  _POSTVALIDATEPASSWORDREQUEST._serialized_end=27677
+  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_start=27680
+  _SINGLEPASSWORDVALIDATIONRESPONSE._serialized_end=27822
+  _GETWORKFLOWREQUEST._serialized_start=27825
+  _GETWORKFLOWREQUEST._serialized_end=28012
+  _LISTWORKFLOWSREQUEST._serialized_start=28015
+  _LISTWORKFLOWSREQUEST._serialized_end=28408
+  _POSTWORKFLOWSREQUEST._serialized_start=28410
+  _POSTWORKFLOWSREQUEST._serialized_end=28524
+  _PATCHWORKFLOWSREQUEST._serialized_start=28527
+  _PATCHWORKFLOWSREQUEST._serialized_end=28658
+  _PATCHWORKFLOWIDSREQUEST._serialized_start=28661
+  _PATCHWORKFLOWIDSREQUEST._serialized_end=28794
+  _DELETEWORKFLOWREQUEST._serialized_start=28796
+  _DELETEWORKFLOWREQUEST._serialized_end=28889
+  _DELETEWORKFLOWSREQUEST._serialized_start=28891
+  _DELETEWORKFLOWSREQUEST._serialized_end=28997
+  _SINGLEWORKFLOWRESPONSE._serialized_start=28999
+  _SINGLEWORKFLOWRESPONSE._serialized_end=29110
+  _MULTIWORKFLOWRESPONSE._serialized_start=29112
+  _MULTIWORKFLOWRESPONSE._serialized_end=29229
+  _POSTWORKFLOWRESULTSREQUEST._serialized_start=29232
+  _POSTWORKFLOWRESULTSREQUEST._serialized_end=29525
+  _POSTWORKFLOWRESULTSRESPONSE._serialized_start=29528
+  _POSTWORKFLOWRESULTSRESPONSE._serialized_end=29744
+  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_start=29747
+  _POSTWORKFLOWRESULTSSIMILARITYREQUEST._serialized_end=30020
+  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_start=30023
+  _POSTWORKFLOWRESULTSSIMILARITYRESPONSE._serialized_end=30165
+  _LISTWORKFLOWVERSIONSREQUEST._serialized_start=30168
+  _LISTWORKFLOWVERSIONSREQUEST._serialized_end=30299
+  _GETWORKFLOWVERSIONREQUEST._serialized_start=30301
+  _GETWORKFLOWVERSIONREQUEST._serialized_end=30427
+  _DELETEWORKFLOWVERSIONSREQUEST._serialized_start=30430
+  _DELETEWORKFLOWVERSIONSREQUEST._serialized_end=30561
+  _PATCHWORKFLOWVERSIONSREQUEST._serialized_start=30564
+  _PATCHWORKFLOWVERSIONSREQUEST._serialized_end=30738
+  _MULTIWORKFLOWVERSIONRESPONSE._serialized_start=30741
+  _MULTIWORKFLOWVERSIONRESPONSE._serialized_end=30880
+  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_start=30883
+  _SINGLEWORKFLOWVERSIONRESPONSE._serialized_end=31016
+  _POSTAPPDUPLICATIONSREQUEST._serialized_start=31019
+  _POSTAPPDUPLICATIONSREQUEST._serialized_end=31152
+  _GETAPPDUPLICATIONREQUEST._serialized_start=31154
+  _GETAPPDUPLICATIONREQUEST._serialized_end=31257
+  _LISTAPPDUPLICATIONSREQUEST._serialized_start=31259
+  _LISTAPPDUPLICATIONSREQUEST._serialized_end=31368
+  _MULTIAPPDUPLICATIONSRESPONSE._serialized_start=31371
+  _MULTIAPPDUPLICATIONSRESPONSE._serialized_end=31502
+  _SINGLEAPPDUPLICATIONRESPONSE._serialized_start=31505
+  _SINGLEAPPDUPLICATIONRESPONSE._serialized_end=31635
+  _POSTTASKSREQUEST._serialized_start=31637
+  _POSTTASKSREQUEST._serialized_end=31739
+  _GETTASKREQUEST._serialized_start=31741
+  _GETTASKREQUEST._serialized_end=31850
+  _LISTTASKSREQUEST._serialized_start=31853
+  _LISTTASKSREQUEST._serialized_end=32091
+  _PATCHTASKSREQUEST._serialized_start=32093
+  _PATCHTASKSREQUEST._serialized_end=32212
+  _DELETETASKSREQUEST._serialized_start=32214
+  _DELETETASKSREQUEST._serialized_end=32296
+  _MULTITASKRESPONSE._serialized_start=32298
+  _MULTITASKRESPONSE._serialized_end=32403
+  _SINGLETASKRESPONSE._serialized_start=32405
+  _SINGLETASKRESPONSE._serialized_end=32504
+  _GETTASKCOUNTREQUEST._serialized_start=32506
+  _GETTASKCOUNTREQUEST._serialized_end=32611
+  _SINGLETASKCOUNTRESPONSE._serialized_start=32614
+  _SINGLETASKCOUNTRESPONSE._serialized_end=32771
+  _POSTLABELORDERSREQUEST._serialized_start=32773
+  _POSTLABELORDERSREQUEST._serialized_end=32894
+  _GETLABELORDERREQUEST._serialized_start=32896
+  _GETLABELORDERREQUEST._serialized_end=32991
+  _LISTLABELORDERSREQUEST._serialized_start=32993
+  _LISTLABELORDERSREQUEST._serialized_end=33098
+  _PATCHLABELORDERSREQUEST._serialized_start=33101
+  _PATCHLABELORDERSREQUEST._serialized_end=33239
+  _DELETELABELORDERSREQUEST._serialized_start=33241
+  _DELETELABELORDERSREQUEST._serialized_end=33329
+  _MULTILABELORDERRESPONSE._serialized_start=33331
+  _MULTILABELORDERRESPONSE._serialized_end=33455
+  _SINGLELABELORDERRESPONSE._serialized_start=33457
+  _SINGLELABELORDERRESPONSE._serialized_end=33575
+  _POSTCOLLECTORSREQUEST._serialized_start=33577
+  _POSTCOLLECTORSREQUEST._serialized_end=33694
+  _PATCHCOLLECTORSREQUEST._serialized_start=33697
+  _PATCHCOLLECTORSREQUEST._serialized_end=33831
+  _DELETECOLLECTORSREQUEST._serialized_start=33833
+  _DELETECOLLECTORSREQUEST._serialized_end=33940
+  _GETCOLLECTORREQUEST._serialized_start=33942
+  _GETCOLLECTORREQUEST._serialized_end=34034
+  _LISTCOLLECTORSREQUEST._serialized_start=34036
+  _LISTCOLLECTORSREQUEST._serialized_end=34140
+  _MULTICOLLECTORRESPONSE._serialized_start=34142
+  _MULTICOLLECTORRESPONSE._serialized_end=34256
+  _SINGLECOLLECTORRESPONSE._serialized_start=34258
+  _SINGLECOLLECTORRESPONSE._serialized_end=34372
+  _POSTSTATVALUESREQUEST._serialized_start=34374
+  _POSTSTATVALUESREQUEST._serialized_end=34492
+  _MULTISTATVALUERESPONSE._serialized_start=34494
+  _MULTISTATVALUERESPONSE._serialized_end=34615
+  _POSTSTATVALUESAGGREGATEREQUEST._serialized_start=34618
+  _POSTSTATVALUESAGGREGATEREQUEST._serialized_end=34776
+  _MULTISTATVALUEAGGREGATERESPONSE._serialized_start=34779
+  _MULTISTATVALUEAGGREGATERESPONSE._serialized_end=34935
+  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_start=34937
+  _POSTTRENDINGMETRICSVIEWREQUEST._serialized_end=35056
+  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_start=35059
+  _LISTTRENDINGMETRICSVIEWSREQUEST._serialized_end=35192
+  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_start=35194
+  _MULTITRENDINGMETRICSVIEWRESPONSE._serialized_end=35320
+  _GETMODULEREQUEST._serialized_start=35322
+  _GETMODULEREQUEST._serialized_end=35435
+  _LISTMODULESREQUEST._serialized_start=35438
+  _LISTMODULESREQUEST._serialized_end=35732
+  _POSTMODULESREQUEST._serialized_start=35734
+  _POSTMODULESREQUEST._serialized_end=35842
+  _PATCHMODULESREQUEST._serialized_start=35844
+  _PATCHMODULESREQUEST._serialized_end=35969
+  _DELETEMODULESREQUEST._serialized_start=35971
+  _DELETEMODULESREQUEST._serialized_end=36055
+  _SINGLEMODULERESPONSE._serialized_start=36057
+  _SINGLEMODULERESPONSE._serialized_end=36162
+  _MULTIMODULERESPONSE._serialized_start=36164
+  _MULTIMODULERESPONSE._serialized_end=36275
+  _GETMODULEVERSIONREQUEST._serialized_start=36277
+  _GETMODULEVERSIONREQUEST._serialized_end=36397
+  _LISTMODULEVERSIONSREQUEST._serialized_start=36399
+  _LISTMODULEVERSIONSREQUEST._serialized_end=36526
+  _POSTMODULEVERSIONSREQUEST._serialized_start=36529
+  _POSTMODULEVERSIONSREQUEST._serialized_end=36678
+  _DELETEMODULEVERSIONSREQUEST._serialized_start=36680
+  _DELETEMODULEVERSIONSREQUEST._serialized_end=36790
+  _SINGLEMODULEVERSIONRESPONSE._serialized_start=36792
+  _SINGLEMODULEVERSIONRESPONSE._serialized_end=36919
+  _MULTIMODULEVERSIONRESPONSE._serialized_start=36922
+  _MULTIMODULEVERSIONRESPONSE._serialized_end=37055
+  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_start=37057
+  _GETINSTALLEDMODULEVERSIONREQUEST._serialized_end=37177
+  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=37179
+  _LISTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=37296
+  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_start=37299
+  _POSTINSTALLEDMODULEVERSIONSREQUEST._serialized_end=37457
+  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_start=37459
+  _POSTINSTALLEDMODULEVERSIONSKEYREQUEST._serialized_end=37584
+  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_start=37586
+  _DELETEINSTALLEDMODULEVERSIONSREQUEST._serialized_end=37686
+  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_start=37689
+  _SINGLEINSTALLEDMODULEVERSIONRESPONSE._serialized_end=37844
+  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_start=37847
+  _MULTIINSTALLEDMODULEVERSIONRESPONSE._serialized_end=38008
+  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_start=38010
+  _LISTNEXTTASKASSIGNMENTSREQUEST._serialized_end=38108
+  _POSTBULKOPERATIONSREQUEST._serialized_start=38111
+  _POSTBULKOPERATIONSREQUEST._serialized_end=38241
+  _LISTBULKOPERATIONSREQUEST._serialized_start=38243
+  _LISTBULKOPERATIONSREQUEST._serialized_end=38351
+  _GETBULKOPERATIONREQUEST._serialized_start=38353
+  _GETBULKOPERATIONREQUEST._serialized_end=38439
+  _CANCELBULKOPERATIONREQUEST._serialized_start=38441
+  _CANCELBULKOPERATIONREQUEST._serialized_end=38531
+  _DELETEBULKOPERATIONREQUEST._serialized_start=38533
+  _DELETEBULKOPERATIONREQUEST._serialized_end=38623
+  _SINGLEBULKOPERATIONSRESPONSE._serialized_start=38626
+  _SINGLEBULKOPERATIONSRESPONSE._serialized_end=38754
+  _MULTIBULKOPERATIONSRESPONSE._serialized_start=38756
+  _MULTIBULKOPERATIONSRESPONSE._serialized_end=38883
+  _PUTTASKASSIGNMENTSREQUEST._serialized_start=38885
+  _PUTTASKASSIGNMENTSREQUEST._serialized_end=38996
+  _LISTINPUTSADDJOBSREQUEST._serialized_start=38998
+  _LISTINPUTSADDJOBSREQUEST._serialized_end=39105
+  _GETINPUTSADDJOBREQUEST._serialized_start=39107
+  _GETINPUTSADDJOBREQUEST._serialized_end=39192
+  _CANCELINPUTSADDJOBREQUEST._serialized_start=39194
+  _CANCELINPUTSADDJOBREQUEST._serialized_end=39282
+  _MULTIINPUTSADDJOBRESPONSE._serialized_start=39285
+  _MULTIINPUTSADDJOBRESPONSE._serialized_end=39416
+  _SINGLEINPUTSADDJOBRESPONSE._serialized_start=39418
+  _SINGLEINPUTSADDJOBRESPONSE._serialized_end=39543
+  _POSTUPLOADSREQUEST._serialized_start=39545
+  _POSTUPLOADSREQUEST._serialized_end=39653
+  _DELETEUPLOADSREQUEST._serialized_start=39655
+  _DELETEUPLOADSREQUEST._serialized_end=39739
+  _LISTUPLOADSREQUEST._serialized_start=39741
+  _LISTUPLOADSREQUEST._serialized_end=39842
+  _GETUPLOADREQUEST._serialized_start=39844
+  _GETUPLOADREQUEST._serialized_end=39930
+  _SINGLEUPLOADRESPONSE._serialized_start=39932
+  _SINGLEUPLOADRESPONSE._serialized_end=40037
+  _MULTIUPLOADRESPONSE._serialized_start=40039
+  _MULTIUPLOADRESPONSE._serialized_end=40144
+  _PUTUPLOADCONTENTPARTSREQUEST._serialized_start=40147
+  _PUTUPLOADCONTENTPARTSREQUEST._serialized_end=40301
+  _POSTINPUTSDATASOURCESREQUEST._serialized_start=40304
+  _POSTINPUTSDATASOURCESREQUEST._serialized_end=40477
+  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_start=40479
+  _GETINPUTSEXTRACTIONJOBREQUEST._serialized_end=40593
+  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_start=40595
+  _LISTINPUTSEXTRACTIONJOBSREQUEST._serialized_end=40709
+  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_start=40712
+  _SINGLEINPUTSEXTRACTIONJOBRESPONSE._serialized_end=40858
+  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_start=40861
+  _MULTIINPUTSEXTRACTIONJOBRESPONSE._serialized_end=41007
+  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_start=41009
+  _CANCELINPUTSEXTRACTIONJOBSREQUEST._serialized_end=41106
+  _POSTINPUTSUPLOADSREQUEST._serialized_start=41108
+  _POSTINPUTSUPLOADSREQUEST._serialized_end=41235
+  _GETRUNNERREQUEST._serialized_start=41237
+  _GETRUNNERREQUEST._serialized_end=41323
+  _LISTRUNNERSREQUEST._serialized_start=41325
+  _LISTRUNNERSREQUEST._serialized_end=41426
+  _POSTRUNNERSREQUEST._serialized_start=41428
+  _POSTRUNNERSREQUEST._serialized_end=41536
+  _DELETERUNNERSREQUEST._serialized_start=41538
+  _DELETERUNNERSREQUEST._serialized_end=41622
+  _SINGLERUNNERRESPONSE._serialized_start=41624
+  _SINGLERUNNERRESPONSE._serialized_end=41729
+  _MULTIRUNNERRESPONSE._serialized_start=41731
+  _MULTIRUNNERRESPONSE._serialized_end=41842
+  _LISTRUNNERITEMSREQUEST._serialized_start=41844
+  _LISTRUNNERITEMSREQUEST._serialized_end=41936
+  _POSTRUNNERITEMOUTPUTSREQUEST._serialized_start=41939
+  _POSTRUNNERITEMOUTPUTSREQUEST._serialized_end=42115
+  _MULTIRUNNERITEMRESPONSE._serialized_start=42117
+  _MULTIRUNNERITEMRESPONSE._serialized_end=42234
+  _RUNNERITEM._serialized_start=42236
+  _RUNNERITEM._serialized_end=42356
+  _RUNNERITEMOUTPUT._serialized_start=42358
+  _RUNNERITEMOUTPUT._serialized_end=42442
+  _MULTIRUNNERITEMOUTPUTRESPONSE._serialized_start=42445
+  _MULTIRUNNERITEMOUTPUTRESPONSE._serialized_end=42588
+  _V2._serialized_start=42706
+  _V2._serialized_end=93282
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -438,14 +438,16 @@
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PER_PAGE_FIELD_NUMBER: builtins.int
     SORT_ASCENDING_FIELD_NUMBER: builtins.int
     SORT_BY_NAME_FIELD_NUMBER: builtins.int
     SORT_BY_MODIFIED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_CREATED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_STAR_COUNT_FIELD_NUMBER: builtins.int
     QUERY_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     FEATURED_ONLY_FIELD_NUMBER: builtins.int
     STARRED_ONLY_FIELD_NUMBER: builtins.int
     ADDITIONAL_FIELDS_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
@@ -461,16 +463,20 @@
     """Sorting opitons:
     Whether to sort in ascending order. If false, will order in descending order.
     """
     sort_by_name: builtins.bool
     """Whether to order by the name"""
     sort_by_modified_at: builtins.bool
     """Whether to order by the modified_at time.
-    If neither sort option is set to true, will sort by modified_at.
+    If none of the sort options is set to true, will sort by modified_at.
     """
+    sort_by_created_at: builtins.bool
+    """Whether to order by the created_at time."""
+    sort_by_star_count: builtins.bool
+    """Whether to order by the number of users stared the app"""
     query: builtins.str
     """Filtering options:
     Query various text fields that can contain the words in the query string
     """
     name: builtins.str
     """Filter by the name of the app. This supports wilcard queries like "gen*" to match "general" as an example.
     Deprecated in favor of query
@@ -487,23 +493,25 @@
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         page: builtins.int = ...,
         per_page: builtins.int = ...,
         sort_ascending: builtins.bool = ...,
         sort_by_name: builtins.bool = ...,
         sort_by_modified_at: builtins.bool = ...,
+        sort_by_created_at: builtins.bool = ...,
+        sort_by_star_count: builtins.bool = ...,
         query: builtins.str = ...,
         name: builtins.str = ...,
         featured_only: builtins.bool = ...,
         starred_only: builtins.bool = ...,
         additional_fields: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "featured_only", b"featured_only", "name", b"name", "page", b"page", "per_page", b"per_page", "query", b"query", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_name", "sort_by_modified_at"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_star_count", b"sort_by_star_count", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "featured_only", b"featured_only", "name", b"name", "page", b"page", "per_page", b"per_page", "query", b"query", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_star_count", b"sort_by_star_count", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_name", "sort_by_modified_at", "sort_by_created_at", "sort_by_star_count"] | None: ...
 
 global___ListAppsRequest = ListAppsRequest
 
 @typing_extensions.final
 class PostAppsRequest(google.protobuf.message.Message):
     """PostAppsRequest"""
 
@@ -2130,38 +2138,61 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PER_PAGE_FIELD_NUMBER: builtins.int
     STARRED_ONLY_FIELD_NUMBER: builtins.int
     ADDITIONAL_FIELDS_FIELD_NUMBER: builtins.int
+    SORT_ASCENDING_FIELD_NUMBER: builtins.int
+    SORT_BY_CREATED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_STAR_COUNT_FIELD_NUMBER: builtins.int
+    SORT_BY_MODIFIED_AT_FIELD_NUMBER: builtins.int
+    BOOKMARK_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     page: builtins.int
     """(optional URL parameter) The page number. Pagination is used to split the results into chunks.
     Defaults to 1.
     """
     per_page: builtins.int
     """(optional URL parameter) The number of results that will be contained in each page. Defaults
     to 128.
     """
     starred_only: builtins.bool
     @property
     def additional_fields(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    sort_ascending: builtins.bool
+    """Sorting opitons:
+    Whether to sort in ascending order. If false, will order in descending order.
+    """
+    sort_by_created_at: builtins.bool
+    """Whether to order by the created_at time."""
+    sort_by_star_count: builtins.bool
+    """Whether to order by the number of users stared the app"""
+    sort_by_modified_at: builtins.bool
+    """If neither sort option is set to true, will sort by modified_at."""
+    bookmark: builtins.bool
+    """Filter datasets by bookmark. If set, only return bookmarked datasets. Otherwise none bookmarked datasets only."""
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         page: builtins.int = ...,
         per_page: builtins.int = ...,
         starred_only: builtins.bool = ...,
         additional_fields: collections.abc.Iterable[builtins.str] | None = ...,
+        sort_ascending: builtins.bool = ...,
+        sort_by_created_at: builtins.bool = ...,
+        sort_by_star_count: builtins.bool = ...,
+        sort_by_modified_at: builtins.bool = ...,
+        bookmark: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "page", b"page", "per_page", b"per_page", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_star_count", b"sort_by_star_count", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "bookmark", b"bookmark", "page", b"page", "per_page", b"per_page", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_star_count", b"sort_by_star_count", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_created_at", "sort_by_star_count", "sort_by_modified_at"] | None: ...
 
 global___ListDatasetsRequest = ListDatasetsRequest
 
 @typing_extensions.final
 class GetDatasetRequest(google.protobuf.message.Message):
     """GetDatasetRequest"""
 
@@ -3190,14 +3221,16 @@
     USER_APP_ID_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PER_PAGE_FIELD_NUMBER: builtins.int
     SORT_ASCENDING_FIELD_NUMBER: builtins.int
     SORT_BY_NAME_FIELD_NUMBER: builtins.int
     SORT_BY_NUM_INPUTS_FIELD_NUMBER: builtins.int
     SORT_BY_MODIFIED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_CREATED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_STAR_COUNT_FIELD_NUMBER: builtins.int
     QUERY_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     FILTER_BY_USER_ID_FIELD_NUMBER: builtins.int
     MODEL_TYPE_ID_FIELD_NUMBER: builtins.int
     TRAINED_ONLY_FIELD_NUMBER: builtins.int
     INPUT_FIELDS_FIELD_NUMBER: builtins.int
     OUTPUT_FIELDS_FIELD_NUMBER: builtins.int
@@ -3205,14 +3238,15 @@
     FEATURED_ONLY_FIELD_NUMBER: builtins.int
     STARRED_ONLY_FIELD_NUMBER: builtins.int
     TOOLKITS_FIELD_NUMBER: builtins.int
     USE_CASES_FIELD_NUMBER: builtins.int
     LANGUAGES_FIELD_NUMBER: builtins.int
     ADDITIONAL_FIELDS_FIELD_NUMBER: builtins.int
     DONT_FETCH_FROM_MAIN_FIELD_NUMBER: builtins.int
+    BOOKMARK_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     page: builtins.int
     """(optional URL parameter) The page number. Pagination is used to split the results into chunks.
     Defaults to 1.
     """
     per_page: builtins.int
@@ -3225,16 +3259,20 @@
     """
     sort_by_name: builtins.bool
     """Whether to order by the name"""
     sort_by_num_inputs: builtins.bool
     """Whether to order by the number of training inputs"""
     sort_by_modified_at: builtins.bool
     """Whether to order by the modified_at time of the latest model version.
-    If neither sort option is set to true, will sort by modified_at.
+    If none of the sort options is set to true, will sort by modified_at.
     """
+    sort_by_created_at: builtins.bool
+    """Whether to order by the created_at"""
+    sort_by_star_count: builtins.bool
+    """Whether to order by count of stars"""
     query: builtins.str
     """Filtering options:
     Query name, description and id fields, that can contain the words in the query string. Does NOT support wildcards - full words only. Supports operators "OR" and "-" as NOT.
     """
     name: builtins.str
     """Filter by the description and id of the model. This supports wildcard queries like "gen*" to match "general" as an example."""
     filter_by_user_id: builtins.bool
@@ -3273,24 +3311,31 @@
     @property
     def additional_fields(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """(optional URL parameter) List of additional fields to be included in the response. Currently supported: all, stars, outputs, presets"""
     dont_fetch_from_main: builtins.bool
     """Old API behavior resulted in returning clarifai main models when calling ListModels while scoped to an app. While we transition
     away from that, we can use this flag to not always fetch clarifai main models, unless that is the app we are explicitly listing for.
     """
+    bookmark: builtins.bool
+    """Filter models by bookmark. If set, only return bookmarked models. Otherwise none bookmarked models only.
+    Note: you can not filter `trained_only` and bookmark at the same time.
+    When filter by bookmark, we will return trained and untrained models.
+    """
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         page: builtins.int = ...,
         per_page: builtins.int = ...,
         sort_ascending: builtins.bool = ...,
         sort_by_name: builtins.bool = ...,
         sort_by_num_inputs: builtins.bool = ...,
         sort_by_modified_at: builtins.bool = ...,
+        sort_by_created_at: builtins.bool = ...,
+        sort_by_star_count: builtins.bool = ...,
         query: builtins.str = ...,
         name: builtins.str = ...,
         filter_by_user_id: builtins.bool = ...,
         model_type_id: builtins.str = ...,
         trained_only: builtins.bool = ...,
         input_fields: collections.abc.Iterable[builtins.str] | None = ...,
         output_fields: collections.abc.Iterable[builtins.str] | None = ...,
@@ -3298,18 +3343,19 @@
         featured_only: builtins.bool = ...,
         starred_only: builtins.bool = ...,
         toolkits: collections.abc.Iterable[builtins.str] | None = ...,
         use_cases: collections.abc.Iterable[builtins.str] | None = ...,
         languages: collections.abc.Iterable[builtins.str] | None = ...,
         additional_fields: collections.abc.Iterable[builtins.str] | None = ...,
         dont_fetch_from_main: builtins.bool = ...,
+        bookmark: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_num_inputs", b"sort_by_num_inputs", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "dont_fetch_from_main", b"dont_fetch_from_main", "featured_only", b"featured_only", "filter_by_user_id", b"filter_by_user_id", "input_fields", b"input_fields", "languages", b"languages", "license", b"license", "model_type_id", b"model_type_id", "name", b"name", "output_fields", b"output_fields", "page", b"page", "per_page", b"per_page", "query", b"query", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_num_inputs", b"sort_by_num_inputs", "starred_only", b"starred_only", "toolkits", b"toolkits", "trained_only", b"trained_only", "use_cases", b"use_cases", "user_app_id", b"user_app_id"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_name", "sort_by_num_inputs", "sort_by_modified_at"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_num_inputs", b"sort_by_num_inputs", "sort_by_star_count", b"sort_by_star_count", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "bookmark", b"bookmark", "dont_fetch_from_main", b"dont_fetch_from_main", "featured_only", b"featured_only", "filter_by_user_id", b"filter_by_user_id", "input_fields", b"input_fields", "languages", b"languages", "license", b"license", "model_type_id", b"model_type_id", "name", b"name", "output_fields", b"output_fields", "page", b"page", "per_page", b"per_page", "query", b"query", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_name", b"sort_by_name", "sort_by_num_inputs", b"sort_by_num_inputs", "sort_by_star_count", b"sort_by_star_count", "starred_only", b"starred_only", "toolkits", b"toolkits", "trained_only", b"trained_only", "use_cases", b"use_cases", "user_app_id", b"user_app_id"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_name", "sort_by_num_inputs", "sort_by_modified_at", "sort_by_created_at", "sort_by_star_count"] | None: ...
 
 global___ListModelsRequest = ListModelsRequest
 
 @typing_extensions.final
 class GetResourceCountsRequest(google.protobuf.message.Message):
     """ResourceCountRequest"""
 
@@ -5877,20 +5923,23 @@
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PER_PAGE_FIELD_NUMBER: builtins.int
     SORT_ASCENDING_FIELD_NUMBER: builtins.int
     SORT_BY_ID_FIELD_NUMBER: builtins.int
     SORT_BY_MODIFIED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_CREATED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_STAR_COUNT_FIELD_NUMBER: builtins.int
     QUERY_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     FEATURED_ONLY_FIELD_NUMBER: builtins.int
     STARRED_ONLY_FIELD_NUMBER: builtins.int
     ADDITIONAL_FIELDS_FIELD_NUMBER: builtins.int
     SEARCH_TERM_FIELD_NUMBER: builtins.int
+    BOOKMARK_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     page: builtins.int
     """(optional URL parameter) The page number. Pagination is used to split the results into chunks.
     Defaults to 1.
     """
     per_page: builtins.int
@@ -5901,16 +5950,20 @@
     """Sorting options:
     Whether to sort in ascending order. If false, will order in descending order.
     """
     sort_by_id: builtins.bool
     """Whether to order by the name"""
     sort_by_modified_at: builtins.bool
     """Whether to order by the modified_at time.
-    If neither sort option is set to true, will sort by modified_at.
+    If none of the sort options is set to true, will sort by modified_at.
     """
+    sort_by_created_at: builtins.bool
+    """Whether to order by the created_at time."""
+    sort_by_star_count: builtins.bool
+    """Whether to order by the number of users stared the workflow"""
     query: builtins.str
     """Query various text fields that can contain the words in the query string."""
     id: builtins.str
     """Filter by the id of the workflow. This supports wilcard queries like "gen*" to match "general" as an example.
     Deprecated in favor of query
     """
     featured_only: builtins.bool
@@ -5918,33 +5971,38 @@
     starred_only: builtins.bool
     """If true, we only return workflows that are starred by the requesting user"""
     @property
     def additional_fields(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """(optional URL parameter) List of additional fields to be included in the response. Currently supported: all, stars"""
     search_term: builtins.str
     """(optional) search_term. Full text and prefix matching on description, id, owner id. Searchable fields may be added"""
+    bookmark: builtins.bool
+    """Filter workflows by bookmark. If set, only return bookmarked workflows. Otherwise none bookmarked workflows only."""
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         page: builtins.int = ...,
         per_page: builtins.int = ...,
         sort_ascending: builtins.bool = ...,
         sort_by_id: builtins.bool = ...,
         sort_by_modified_at: builtins.bool = ...,
+        sort_by_created_at: builtins.bool = ...,
+        sort_by_star_count: builtins.bool = ...,
         query: builtins.str = ...,
         id: builtins.str = ...,
         featured_only: builtins.bool = ...,
         starred_only: builtins.bool = ...,
         additional_fields: collections.abc.Iterable[builtins.str] | None = ...,
         search_term: builtins.str = ...,
+        bookmark: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_id", b"sort_by_id", "sort_by_modified_at", b"sort_by_modified_at", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "featured_only", b"featured_only", "id", b"id", "page", b"page", "per_page", b"per_page", "query", b"query", "search_term", b"search_term", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_id", b"sort_by_id", "sort_by_modified_at", b"sort_by_modified_at", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_id", "sort_by_modified_at"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_id", b"sort_by_id", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_star_count", b"sort_by_star_count", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "bookmark", b"bookmark", "featured_only", b"featured_only", "id", b"id", "page", b"page", "per_page", b"per_page", "query", b"query", "search_term", b"search_term", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_id", b"sort_by_id", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_star_count", b"sort_by_star_count", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_id", "sort_by_modified_at", "sort_by_created_at", "sort_by_star_count"] | None: ...
 
 global___ListWorkflowsRequest = ListWorkflowsRequest
 
 @typing_extensions.final
 class PostWorkflowsRequest(google.protobuf.message.Message):
     """PostWorkflowsRequest"""
 
@@ -7427,38 +7485,61 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USER_APP_ID_FIELD_NUMBER: builtins.int
     PAGE_FIELD_NUMBER: builtins.int
     PER_PAGE_FIELD_NUMBER: builtins.int
     STARRED_ONLY_FIELD_NUMBER: builtins.int
     ADDITIONAL_FIELDS_FIELD_NUMBER: builtins.int
+    SORT_ASCENDING_FIELD_NUMBER: builtins.int
+    SORT_BY_CREATED_AT_FIELD_NUMBER: builtins.int
+    SORT_BY_STAR_COUNT_FIELD_NUMBER: builtins.int
+    SORT_BY_MODIFIED_AT_FIELD_NUMBER: builtins.int
+    BOOKMARK_FIELD_NUMBER: builtins.int
     @property
     def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
     page: builtins.int
     """(optional URL parameter) The page number. Pagination is used to split the results into chunks.
     Defaults to 1.
     """
     per_page: builtins.int
     """(optional URL parameter) The number of results that will be contained in each page. Defaults
     to 128.
     """
     starred_only: builtins.bool
     @property
     def additional_fields(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    sort_ascending: builtins.bool
+    """Sorting opitons:
+    Whether to sort in ascending order. If false, will order in descending order.
+    """
+    sort_by_created_at: builtins.bool
+    """Whether to order by the created_at time."""
+    sort_by_star_count: builtins.bool
+    """Whether to order by the number of users stared the app"""
+    sort_by_modified_at: builtins.bool
+    """If neither sort option is set to true, will sort by modified_at."""
+    bookmark: builtins.bool
+    """Filter modules by bookmark. If set, only return bookmarked modules. Otherwise none bookmarked modules only."""
     def __init__(
         self,
         *,
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         page: builtins.int = ...,
         per_page: builtins.int = ...,
         starred_only: builtins.bool = ...,
         additional_fields: collections.abc.Iterable[builtins.str] | None = ...,
+        sort_ascending: builtins.bool = ...,
+        sort_by_created_at: builtins.bool = ...,
+        sort_by_star_count: builtins.bool = ...,
+        sort_by_modified_at: builtins.bool = ...,
+        bookmark: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "page", b"page", "per_page", b"per_page", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_star_count", b"sort_by_star_count", "user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["additional_fields", b"additional_fields", "bookmark", b"bookmark", "page", b"page", "per_page", b"per_page", "sort_ascending", b"sort_ascending", "sort_by", b"sort_by", "sort_by_created_at", b"sort_by_created_at", "sort_by_modified_at", b"sort_by_modified_at", "sort_by_star_count", b"sort_by_star_count", "starred_only", b"starred_only", "user_app_id", b"user_app_id"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sort_by", b"sort_by"]) -> typing_extensions.Literal["sort_by_created_at", "sort_by_star_count", "sort_by_modified_at"] | None: ...
 
 global___ListModulesRequest = ListModulesRequest
 
 @typing_extensions.final
 class PostModulesRequest(google.protobuf.message.Message):
     """PostModulesRequest"""
 
@@ -8603,7 +8684,296 @@
         user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
         inputs_uploads: collections.abc.Iterable[proto.clarifai.api.resources_pb2.InputsUpload] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["inputs_uploads", b"inputs_uploads", "user_app_id", b"user_app_id"]) -> None: ...
 
 global___PostInputsUploadsRequest = PostInputsUploadsRequest
+
+@typing_extensions.final
+class GetRunnerRequest(google.protobuf.message.Message):
+    """GetRunnerRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    RUNNER_ID_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    runner_id: builtins.str
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        runner_id: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["runner_id", b"runner_id", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___GetRunnerRequest = GetRunnerRequest
+
+@typing_extensions.final
+class ListRunnersRequest(google.protobuf.message.Message):
+    """ListRunnersRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    PAGE_FIELD_NUMBER: builtins.int
+    PER_PAGE_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    page: builtins.int
+    """(optional URL parameter) The page number. Pagination is used to split the results into chunks.
+    Defaults to 1.
+    """
+    per_page: builtins.int
+    """(optional URL parameter) The number of results that will be contained in each page. Defaults
+    to 128.
+    """
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        page: builtins.int = ...,
+        per_page: builtins.int = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["page", b"page", "per_page", b"per_page", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___ListRunnersRequest = ListRunnersRequest
+
+@typing_extensions.final
+class PostRunnersRequest(google.protobuf.message.Message):
+    """PostRunnersRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    RUNNERS_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    @property
+    def runners(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.Runner]:
+        """This allows you to create one or more runner by posting it to the API."""
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        runners: collections.abc.Iterable[proto.clarifai.api.resources_pb2.Runner] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["runners", b"runners", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___PostRunnersRequest = PostRunnersRequest
+
+@typing_extensions.final
+class DeleteRunnersRequest(google.protobuf.message.Message):
+    """Request to delete several things by the list of ids."""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    IDS_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    @property
+    def ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        ids: collections.abc.Iterable[builtins.str] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ids", b"ids", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___DeleteRunnersRequest = DeleteRunnersRequest
+
+@typing_extensions.final
+class SingleRunnerResponse(google.protobuf.message.Message):
+    """SingleRunnerResponse"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STATUS_FIELD_NUMBER: builtins.int
+    RUNNER_FIELD_NUMBER: builtins.int
+    @property
+    def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
+    @property
+    def runner(self) -> proto.clarifai.api.resources_pb2.Runner: ...
+    def __init__(
+        self,
+        *,
+        status: proto.clarifai.api.status.status_pb2.Status | None = ...,
+        runner: proto.clarifai.api.resources_pb2.Runner | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["runner", b"runner", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["runner", b"runner", "status", b"status"]) -> None: ...
+
+global___SingleRunnerResponse = SingleRunnerResponse
+
+@typing_extensions.final
+class MultiRunnerResponse(google.protobuf.message.Message):
+    """MultiRunnerResponse"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STATUS_FIELD_NUMBER: builtins.int
+    RUNNERS_FIELD_NUMBER: builtins.int
+    @property
+    def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
+    @property
+    def runners(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[proto.clarifai.api.resources_pb2.Runner]: ...
+    def __init__(
+        self,
+        *,
+        status: proto.clarifai.api.status.status_pb2.Status | None = ...,
+        runners: collections.abc.Iterable[proto.clarifai.api.resources_pb2.Runner] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["runners", b"runners", "status", b"status"]) -> None: ...
+
+global___MultiRunnerResponse = MultiRunnerResponse
+
+@typing_extensions.final
+class ListRunnerItemsRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    RUNNER_ID_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    runner_id: builtins.str
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        runner_id: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["runner_id", b"runner_id", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___ListRunnerItemsRequest = ListRunnerItemsRequest
+
+@typing_extensions.final
+class PostRunnerItemOutputsRequest(google.protobuf.message.Message):
+    """PostRunnerItemOutputsRequest"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    USER_APP_ID_FIELD_NUMBER: builtins.int
+    RUNNER_ID_FIELD_NUMBER: builtins.int
+    ITEM_ID_FIELD_NUMBER: builtins.int
+    RUNNER_ITEM_OUTPUTS_FIELD_NUMBER: builtins.int
+    @property
+    def user_app_id(self) -> proto.clarifai.api.resources_pb2.UserAppIDSet: ...
+    runner_id: builtins.str
+    item_id: builtins.str
+    @property
+    def runner_item_outputs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RunnerItemOutput]:
+        """This allows you to create one or more runner by posting it to the API."""
+    def __init__(
+        self,
+        *,
+        user_app_id: proto.clarifai.api.resources_pb2.UserAppIDSet | None = ...,
+        runner_id: builtins.str = ...,
+        item_id: builtins.str = ...,
+        runner_item_outputs: collections.abc.Iterable[global___RunnerItemOutput] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_app_id", b"user_app_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["item_id", b"item_id", "runner_id", b"runner_id", "runner_item_outputs", b"runner_item_outputs", "user_app_id", b"user_app_id"]) -> None: ...
+
+global___PostRunnerItemOutputsRequest = PostRunnerItemOutputsRequest
+
+@typing_extensions.final
+class MultiRunnerItemResponse(google.protobuf.message.Message):
+    """MultiRunnerItemResponse"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STATUS_FIELD_NUMBER: builtins.int
+    ITEMS_FIELD_NUMBER: builtins.int
+    @property
+    def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
+    @property
+    def items(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RunnerItem]: ...
+    def __init__(
+        self,
+        *,
+        status: proto.clarifai.api.status.status_pb2.Status | None = ...,
+        items: collections.abc.Iterable[global___RunnerItem] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["items", b"items", "status", b"status"]) -> None: ...
+
+global___MultiRunnerItemResponse = MultiRunnerItemResponse
+
+@typing_extensions.final
+class RunnerItem(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ID_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    POST_MODEL_OUTPUTS_REQUEST_FIELD_NUMBER: builtins.int
+    id: builtins.str
+    """A UUID hash for this work item."""
+    description: builtins.str
+    """A description of the work to be done in case needed for UIs."""
+    @property
+    def post_model_outputs_request(self) -> global___PostModelOutputsRequest:
+        """TODO(zeiler): make these options a oneof.
+        first work to do would be an inference runner.
+        training request next.
+        """
+    def __init__(
+        self,
+        *,
+        id: builtins.str = ...,
+        description: builtins.str = ...,
+        post_model_outputs_request: global___PostModelOutputsRequest | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["post_model_outputs_request", b"post_model_outputs_request"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "id", b"id", "post_model_outputs_request", b"post_model_outputs_request"]) -> None: ...
+
+global___RunnerItem = RunnerItem
+
+@typing_extensions.final
+class RunnerItemOutput(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    MULTI_OUTPUT_RESPONSE_FIELD_NUMBER: builtins.int
+    @property
+    def multi_output_response(self) -> global___MultiOutputResponse:
+        """The output of the first task type.
+        TODO(zeiler): should the interface be more like pairs of things wiht request/response in one "item"?
+        """
+    def __init__(
+        self,
+        *,
+        multi_output_response: global___MultiOutputResponse | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["multi_output_response", b"multi_output_response"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["multi_output_response", b"multi_output_response"]) -> None: ...
+
+global___RunnerItemOutput = RunnerItemOutput
+
+@typing_extensions.final
+class MultiRunnerItemOutputResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    STATUS_FIELD_NUMBER: builtins.int
+    RUNNER_ITEM_OUTPUTS_FIELD_NUMBER: builtins.int
+    @property
+    def status(self) -> proto.clarifai.api.status.status_pb2.Status: ...
+    @property
+    def runner_item_outputs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RunnerItemOutput]: ...
+    def __init__(
+        self,
+        *,
+        status: proto.clarifai.api.status.status_pb2.Status | None = ...,
+        runner_item_outputs: collections.abc.Iterable[global___RunnerItemOutput] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["runner_item_outputs", b"runner_item_outputs", "status", b"status"]) -> None: ...
+
+global___MultiRunnerItemOutputResponse = MultiRunnerItemOutputResponse
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/service_pb2_grpc.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1065,14 +1065,44 @@
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsExtractionJobResponse),
                 )
         self.PostInputsUploads = channel.unary_unary(
                 '/clarifai.api.V2/PostInputsUploads',
                 request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostInputsUploadsRequest.SerializeToString,
                 response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsAddJobResponse),
                 )
+        self.GetRunner = channel.unary_unary(
+                '/clarifai.api.V2/GetRunner',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetRunnerRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.SingleRunnerResponse),
+                )
+        self.ListRunners = channel.unary_unary(
+                '/clarifai.api.V2/ListRunners',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListRunnersRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerResponse),
+                )
+        self.PostRunners = channel.unary_unary(
+                '/clarifai.api.V2/PostRunners',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostRunnersRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerResponse),
+                )
+        self.DeleteRunners = channel.unary_unary(
+                '/clarifai.api.V2/DeleteRunners',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.DeleteRunnersRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse),
+                )
+        self.ListRunnerItems = channel.unary_unary(
+                '/clarifai.api.V2/ListRunnerItems',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListRunnerItemsRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerItemResponse),
+                )
+        self.PostRunnerItemOutputs = channel.unary_unary(
+                '/clarifai.api.V2/PostRunnerItemOutputs',
+                request_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostRunnerItemOutputsRequest.SerializeToString,
+                response_deserializer=wrap_response_deserializer(proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerItemOutputResponse),
+                )
 
 
 class V2Servicer(object):
     """
     Note: this is based on the google api format defined here. Please
     read this before contributing to this file and other *.proto files
     for the API.
@@ -2608,14 +2638,56 @@
         Associated inputs-add-job contains an upload id which should be completed through `PutUploadContentParts` endpoint.
         Completing the upload will automatically begin unpacking the archive and uploading the contents as inputs.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetRunner(self, request, context):
+        """Get a specific runner from an app.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListRunners(self, request, context):
+        """List all the runners in community, by user or by app.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def PostRunners(self, request, context):
+        """Add a runners to an app.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteRunners(self, request, context):
+        """Delete multiple runners in one request.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListRunnerItems(self, request, context):
+        """List items for the remote runner to work on.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def PostRunnerItemOutputs(self, request, context):
+        """Post back outputs from remote runners
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_V2Servicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListConceptRelations': grpc.unary_unary_rpc_method_handler(
                     servicer.ListConceptRelations,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListConceptRelationsRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiConceptRelationResponse.SerializeToString,
@@ -3646,14 +3718,44 @@
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsExtractionJobResponse.SerializeToString,
             ),
             'PostInputsUploads': grpc.unary_unary_rpc_method_handler(
                     servicer.PostInputsUploads,
                     request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostInputsUploadsRequest.FromString,
                     response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsAddJobResponse.SerializeToString,
             ),
+            'GetRunner': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetRunner,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.GetRunnerRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.SingleRunnerResponse.SerializeToString,
+            ),
+            'ListRunners': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListRunners,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListRunnersRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerResponse.SerializeToString,
+            ),
+            'PostRunners': grpc.unary_unary_rpc_method_handler(
+                    servicer.PostRunners,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostRunnersRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerResponse.SerializeToString,
+            ),
+            'DeleteRunners': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteRunners,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.DeleteRunnersRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse.SerializeToString,
+            ),
+            'ListRunnerItems': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListRunnerItems,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.ListRunnerItemsRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerItemResponse.SerializeToString,
+            ),
+            'PostRunnerItemOutputs': grpc.unary_unary_rpc_method_handler(
+                    servicer.PostRunnerItemOutputs,
+                    request_deserializer=proto_dot_clarifai_dot_api_dot_service__pb2.PostRunnerItemOutputsRequest.FromString,
+                    response_serializer=proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerItemOutputResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'clarifai.api.V2', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -7192,7 +7294,109 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PostInputsUploads',
             proto_dot_clarifai_dot_api_dot_service__pb2.PostInputsUploadsRequest.SerializeToString,
             proto_dot_clarifai_dot_api_dot_service__pb2.MultiInputsAddJobResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetRunner(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/GetRunner',
+            proto_dot_clarifai_dot_api_dot_service__pb2.GetRunnerRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.SingleRunnerResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListRunners(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/ListRunners',
+            proto_dot_clarifai_dot_api_dot_service__pb2.ListRunnersRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def PostRunners(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PostRunners',
+            proto_dot_clarifai_dot_api_dot_service__pb2.PostRunnersRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteRunners(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/DeleteRunners',
+            proto_dot_clarifai_dot_api_dot_service__pb2.DeleteRunnersRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_status_dot_status__pb2.BaseResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListRunnerItems(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/ListRunnerItems',
+            proto_dot_clarifai_dot_api_dot_service__pb2.ListRunnerItemsRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerItemResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def PostRunnerItemOutputs(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/clarifai.api.V2/PostRunnerItemOutputs',
+            proto_dot_clarifai_dot_api_dot_service__pb2.PostRunnerItemOutputsRequest.SerializeToString,
+            proto_dot_clarifai_dot_api_dot_service__pb2.MultiRunnerItemOutputResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_code_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+proto/clarifai/api/status/status_code.proto\x12\x13\x63larifai.api.status*\xccS\n\nStatusCode\x12\x08\n\x04ZERO\x10\x00\x12\x0c\n\x07SUCCESS\x10\x90N\x12\x11\n\x0cMIXED_STATUS\x10\x9aN\x12\x0c\n\x07\x46\x41ILURE\x10\xa4N\x12\x0e\n\tTRY_AGAIN\x10\xaeN\x12\x14\n\x0fNOT_IMPLEMENTED\x10\xb8N\x12\n\n\x05MOVED\x10\xc2N\x12\x18\n\x13\x43ONN_ACCOUNT_ISSUES\x10\xf8U\x12\x1b\n\x12\x43ONN_TOKEN_INVALID\x10\xf9U\x1a\x02\x08\x01\x12\x1d\n\x18\x43ONN_CREDENTIALS_INVALID\x10\xfaU\x12\x1d\n\x18\x43ONN_EXCEED_HOURLY_LIMIT\x10\xfbU\x12\x1e\n\x19\x43ONN_EXCEED_MONTHLY_LIMIT\x10\xfcU\x12\x13\n\x0e\x43ONN_THROTTLED\x10\xfdU\x12\x18\n\x13\x43ONN_EXCEEDS_LIMITS\x10\xfeU\x12\x1d\n\x18\x43ONN_INSUFFICIENT_SCOPES\x10\xffU\x12\x15\n\x10\x43ONN_KEY_INVALID\x10\x80V\x12\x17\n\x12\x43ONN_KEY_NOT_FOUND\x10\x81V\x12\x1c\n\x17\x43ONN_BAD_REQUEST_FORMAT\x10\xdcV\x12\x18\n\x13\x43ONN_DOES_NOT_EXIST\x10\xddV\x12\x19\n\x14\x43ONN_INVALID_REQUEST\x10\xdeV\x12\x1c\n\x17\x43ONN_METHOD_NOT_ALLOWED\x10\xdfV\x12\x19\n\x14\x43ONN_NO_GDPR_CONSENT\x10\xe0V\x12\x1e\n\x19\x43ONN_AUTH_METHOD_DISABLED\x10\xc0W\x12\x13\n\rMODEL_TRAINED\x10\xec\xa4\x01\x12\x14\n\x0eMODEL_TRAINING\x10\xed\xa4\x01\x12\x15\n\x0fMODEL_UNTRAINED\x10\xee\xa4\x01\x12\x1f\n\x19MODEL_QUEUED_FOR_TRAINING\x10\xef\xa4\x01\x12\x15\n\x0fMODEL_UPLOADING\x10\xf0\xa4\x01\x12\x1c\n\x16MODEL_UPLOADING_FAILED\x10\xf1\xa4\x01\x12\x1b\n\x15MODEL_TRAINING_FAILED\x10\xf2\xa4\x01\x12\x1c\n\x16MODEL_TRAINING_NO_DATA\x10\xf6\xa4\x01\x12!\n\x1bMODEL_TRAINING_NO_POSITIVES\x10\xf7\xa4\x01\x12*\n$MODEL_TRAINING_ONE_VS_N_SINGLE_CLASS\x10\xf8\xa4\x01\x12\x1e\n\x18MODEL_TRAINING_TIMED_OUT\x10\xf9\xa4\x01\x12\"\n\x1cMODEL_TRAINING_WAITING_ERROR\x10\xfa\xa4\x01\x12\"\n\x1cMODEL_TRAINING_UNKNOWN_ERROR\x10\xfb\xa4\x01\x12&\n\x1cMODEL_TRAINING_MSG_REDELIVER\x10\xfc\xa4\x01\x1a\x02\x08\x01\x12&\n MODEL_TRAINING_INSUFFICIENT_DATA\x10\xfd\xa4\x01\x12#\n\x1dMODEL_TRAINING_INVALID_PARAMS\x10\xfe\xa4\x01\x12\x34\n.MODEL_TRAINING_INVALID_DATA_TOLERANCE_EXCEEDED\x10\xff\xa4\x01\x12\x1a\n\x14MODEL_MODIFY_SUCCESS\x10\x9e\xa5\x01\x12\x1a\n\x14MODEL_MODIFY_PENDING\x10\x9f\xa5\x01\x12\x19\n\x13MODEL_MODIFY_FAILED\x10\xa0\xa5\x01\x12\x1a\n\x14MODEL_DOES_NOT_EXIST\x10\xd0\xa5\x01\x12\x1d\n\x17MODEL_PERMISSION_DENIED\x10\xd1\xa5\x01\x12\x1c\n\x16MODEL_INVALID_ARGUMENT\x10\xd2\xa5\x01\x12\x1b\n\x15MODEL_INVALID_REQUEST\x10\xd3\xa5\x01\x12\x15\n\x0fMODEL_EVALUATED\x10\xb4\xa6\x01\x12\x16\n\x10MODEL_EVALUATING\x10\xb5\xa6\x01\x12\x19\n\x13MODEL_NOT_EVALUATED\x10\xb6\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_EVALUATION\x10\xb7\xa6\x01\x12 \n\x1aMODEL_EVALUATION_TIMED_OUT\x10\xbe\xa6\x01\x12$\n\x1eMODEL_EVALUATION_WAITING_ERROR\x10\xbf\xa6\x01\x12$\n\x1eMODEL_EVALUATION_UNKNOWN_ERROR\x10\xc0\xa6\x01\x12\x1d\n\x17MODEL_PREDICTION_FAILED\x10\xc1\xa6\x01\x12(\n\x1eMODEL_EVALUATION_MSG_REDELIVER\x10\xc2\xa6\x01\x1a\x02\x08\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_LABELS\x10\xc3\xa6\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_INPUTS\x10\xc4\xa6\x01\x12\x1d\n\x17MODEL_EVALUATION_FAILED\x10\xc5\xa6\x01\x12\x1d\n\x17MODEL_DEPLOYMENT_FAILED\x10\xe6\xa6\x01\x12\x15\n\x0fMODEL_DEPLOYING\x10\xe7\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_DEPLOYMENT\x10\xe8\xa6\x01\x12\x18\n\x12MODEL_NOT_DEPLOYED\x10\xe9\xa6\x01\x12&\n MODEL_REFERENCE_INVALID_ARGUMENT\x10\x98\xa7\x01\x12*\n$MODEL_EXAMPLE_INPUT_INVALID_ARGUMENT\x10\xac\xa7\x01\x12 \n\x1aWORKFLOW_NO_MATCHING_INPUT\x10\xf1\xab\x01\x12$\n\x1eWORKFLOW_REQUIRE_TRAINED_MODEL\x10\xf2\xab\x01\x12\x18\n\x12WORKFLOW_DUPLICATE\x10\xd4\xac\x01\x12!\n\x1bWORKFLOW_UNSUPPORTED_FORMAT\x10\xd5\xac\x01\x12\x1d\n\x17WORKFLOW_DOES_NOT_EXIST\x10\xd6\xac\x01\x12 \n\x1aWORKFLOW_PERMISSION_DENIED\x10\xd7\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_ARGUMENT\x10\xd8\xac\x01\x12\x1d\n\x17WORKFLOW_INVALID_RECIPE\x10\xd9\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_TEMPLATE\x10\xda\xac\x01\x12\x1c\n\x16WORKFLOW_INVALID_GRAPH\x10\xdb\xac\x01\x12\x1f\n\x19WORKFLOW_INTERNAL_FAILURE\x10\xdc\xac\x01\x12\x1e\n\x18WORKFLOW_INVALID_REQUEST\x10\xd7\xb3\x01\x12\x1d\n\x17WORKFLOW_MODIFY_SUCCESS\x10\x86\xad\x01\x12\x1d\n\x17WORKFLOW_MODIFY_PENDING\x10\x87\xad\x01\x12\x1c\n\x16WORKFLOW_MODIFY_FAILED\x10\x88\xad\x01\x12\x1d\n\x17WORKFLOW_REINDEX_FAILED\x10\x89\xad\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_SUCCESS\x10\xee\xb4\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_PENDING\x10\xef\xb4\x01\x12\x1b\n\x15\x43ONCEPT_MODIFY_FAILED\x10\xf0\xb4\x01\x12\x18\n\x12\x41NNOTATION_SUCCESS\x10\xd6\xbc\x01\x12\x18\n\x12\x41NNOTATION_PENDING\x10\xd7\xbc\x01\x12\x17\n\x11\x41NNOTATION_FAILED\x10\xd8\xbc\x01\x12\x1f\n\x19\x41NNOTATION_UNKNOWN_STATUS\x10\xda\xbc\x01\x12!\n\x1b\x41NNOTATION_INVALID_ARGUMENT\x10\xdb\xbc\x01\x12\"\n\x1c\x41NNOTATION_PERMISSION_DENIED\x10\xdc\xbc\x01\x12 \n\x1a\x41NNOTATION_AWAITING_REVIEW\x10\xdd\xbc\x01\x12*\n$ANNOTATION_AWAITING_CONSENSUS_REVIEW\x10\xdf\xbc\x01\x12\x1e\n\x18\x41NNOTATION_REVIEW_DENIED\x10\xde\xbc\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_SUCCESS\x10\xba\xbd\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_PENDING\x10\xbb\xbd\x01\x12\x1e\n\x18\x41NNOTATION_MODIFY_FAILED\x10\xbc\xbd\x01\x12&\n METADATA_INVALID_PATCH_ARGUMENTS\x10\xc4\xc2\x01\x12\x1c\n\x16METADATA_PARSING_ISSUE\x10\xc5\xc2\x01\x12!\n\x1bMETADATA_MANIPULATION_ISSUE\x10\xc6\xc2\x01\x12\x1c\n\x16TRAINER_JOB_STATE_NONE\x10\xa8\xc3\x01\x12\x1e\n\x18TRAINER_JOB_STATE_QUEUED\x10\xa9\xc3\x01\x12\x1f\n\x19TRAINER_JOB_STATE_RUNNING\x10\xaa\xc3\x01\x12 \n\x1aTRAINER_JOB_STATE_COMPLETE\x10\xab\xc3\x01\x12\x1d\n\x17TRAINER_JOB_STATE_ERROR\x10\xac\xc3\x01\x12\x17\n\x11\x44\x41TA_DUMP_SUCCESS\x10\xbe\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_PENDING\x10\xbf\xc4\x01\x12\x16\n\x10\x44\x41TA_DUMP_FAILED\x10\xc0\xc4\x01\x12\x1b\n\x15\x44\x41TA_DUMP_IN_PROGRESS\x10\xc1\xc4\x01\x12\x1b\n\x11\x44\x41TA_DUMP_NO_DATA\x10\xc2\xc4\x01\x1a\x02\x08\x01\x12 \n\x1a\x44\x41TA_DUMP_UNEXPECTED_ERROR\x10\xc3\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_SUCCESS\x10\xd2\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_PENDING\x10\xd3\xc4\x01\x12\x1d\n\x17\x44\x41TA_DUMP_EXPORT_FAILED\x10\xd4\xc4\x01\x12\"\n\x1c\x44\x41TA_DUMP_EXPORT_IN_PROGRESS\x10\xd5\xc4\x01\x12\'\n!DATA_DUMP_EXPORT_UNEXPECTED_ERROR\x10\xd6\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_SUCCESS\x10\xf0\xc4\x01\x12\x1c\n\x16\x41PP_DUPLICATION_FAILED\x10\xf1\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_PENDING\x10\xf2\xc4\x01\x12!\n\x1b\x41PP_DUPLICATION_IN_PROGRESS\x10\xf3\xc4\x01\x12%\n\x1f\x41PP_DUPLICATION_INVALID_REQUEST\x10\xf4\xc4\x01\x12\x1b\n\x15MODULE_DOES_NOT_EXIST\x10\xd4\xc5\x01\x12\x1e\n\x18MODULE_PERMISSION_DENIED\x10\xd5\xc5\x01\x12\x1d\n\x17MODULE_INVALID_ARGUMENT\x10\xd6\xc5\x01\x12\x1c\n\x16MODULE_INVALID_REQUEST\x10\xd7\xc5\x01\x12\x1c\n\x16\x42ULK_OPERATION_SUCCESS\x10\xb8\xc6\x01\x12\x1b\n\x15\x42ULK_OPERATION_FAILED\x10\xb9\xc6\x01\x12\x1c\n\x16\x42ULK_OPERATION_PENDING\x10\xba\xc6\x01\x12 \n\x1a\x42ULK_OPERATION_IN_PROGRESS\x10\xbb\xc6\x01\x12$\n\x1e\x42ULK_OPERATION_INVALID_REQUEST\x10\xbc\xc6\x01\x12\x1e\n\x18\x42ULK_OPERATION_CANCELLED\x10\xbd\xc6\x01\x12%\n\x1f\x42ULK_OPERATION_UNEXPECTED_ERROR\x10\xbe\xc6\x01\x12\x1c\n\x16INPUT_DOWNLOAD_SUCCESS\x10\xb0\xea\x01\x12\x1c\n\x16INPUT_DOWNLOAD_PENDING\x10\xb1\xea\x01\x12\x1b\n\x15INPUT_DOWNLOAD_FAILED\x10\xb2\xea\x01\x12 \n\x1aINPUT_DOWNLOAD_IN_PROGRESS\x10\xb3\xea\x01\x12 \n\x1aINPUT_STATUS_UPDATE_FAILED\x10\xb4\xea\x01\x12\x19\n\x13INPUT_DELETE_FAILED\x10\xb5\xea\x01\x12\x15\n\x0fINPUT_DUPLICATE\x10\x94\xeb\x01\x12\x1e\n\x18INPUT_UNSUPPORTED_FORMAT\x10\x95\xeb\x01\x12\x1a\n\x14INPUT_DOES_NOT_EXIST\x10\x96\xeb\x01\x12\x1d\n\x17INPUT_PERMISSION_DENIED\x10\x97\xeb\x01\x12\x1c\n\x16INPUT_INVALID_ARGUMENT\x10\x98\xeb\x01\x12\x16\n\x10INPUT_OVER_LIMIT\x10\x99\xeb\x01\x12\x17\n\x11INPUT_INVALID_URL\x10\x9a\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_SUCCESS\x10\xf8\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_PENDING\x10\xf9\xeb\x01\x12\x19\n\x13INPUT_MODIFY_FAILED\x10\xfb\xeb\x01\x12\x1f\n\x19INPUT_STORAGE_HOST_FAILED\x10\x82\xec\x01\x12\x1d\n\x17\x41LL_INPUT_INVALID_BYTES\x10\xdc\xec\x01\x12\x1b\n\x15INPUT_CLUSTER_SUCCESS\x10\xc0\xed\x01\x12\x1b\n\x15INPUT_CLUSTER_PENDING\x10\xc1\xed\x01\x12\x1a\n\x14INPUT_CLUSTER_FAILED\x10\xc2\xed\x01\x12\x1f\n\x19INPUT_CLUSTER_IN_PROGRESS\x10\xc3\xed\x01\x12\x1b\n\x15INPUT_REINDEX_SUCCESS\x10\xa4\xee\x01\x12\x1b\n\x15INPUT_REINDEX_PENDING\x10\xa5\xee\x01\x12\x1a\n\x14INPUT_REINDEX_FAILED\x10\xa6\xee\x01\x12\x1f\n\x19INPUT_REINDEX_IN_PROGRESS\x10\xa7\xee\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_SUCCESS\x10\x98\xf2\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_PENDING\x10\x99\xf2\x01\x12!\n\x1bINPUT_VIDEO_DOWNLOAD_FAILED\x10\x9a\xf2\x01\x12\x1b\n\x15INPUT_VIDEO_DUPLICATE\x10\xfc\xf2\x01\x12$\n\x1eINPUT_VIDEO_UNSUPPORTED_FORMAT\x10\xfd\xf2\x01\x12 \n\x1aINPUT_VIDEO_DOES_NOT_EXIST\x10\xfe\xf2\x01\x12#\n\x1dINPUT_VIDEO_PERMISSION_DENIED\x10\xff\xf2\x01\x12\"\n\x1cINPUT_VIDEO_INVALID_ARGUMENT\x10\x80\xf3\x01\x12\x1c\n\x16INPUT_VIDEO_OVER_LIMIT\x10\x81\xf3\x01\x12\x1d\n\x17INPUT_VIDEO_INVALID_URL\x10\x82\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_SUCCESS\x10\xe0\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_PENDING\x10\xe1\xf3\x01\x12\x1f\n\x19INPUT_VIDEO_MODIFY_FAILED\x10\xe3\xf3\x01\x12%\n\x1fINPUT_VIDEO_STORAGE_HOST_FAILED\x10\xea\xf3\x01\x12$\n\x1e\x41LL_INPUT_VIDEOS_INVALID_BYTES\x10\xc4\xf4\x01\x12$\n\x1eINPUT_VIDEO_PROCESSING_SUCCESS\x10\xa8\xf5\x01\x12$\n\x1eINPUT_VIDEO_PROCESSING_PENDING\x10\xb2\xf5\x01\x12#\n\x1dINPUT_VIDEO_PROCESSING_FAILED\x10\xbc\xf5\x01\x12\'\n!INPUT_VIDEO_STORAGE_INCONSISTENCY\x10\xc6\xf5\x01\x12!\n\x1bINPUT_VIDEO_STORAGE_FAILURE\x10\xd0\xf5\x01\x12(\n\"INPUT_VIDEO_URL_GENERATION_FAILURE\x10\xda\xf5\x01\x12\x1d\n\x17INPUT_CONNECTION_FAILED\x10\xbc\xb8\x02\x12&\n REQUEST_DISABLED_FOR_MAINTENANCE\x10\xbd\xb8\x02\x12/\n%INPUT_WRITES_DISABLED_FOR_MAINTENANCE\x10\xbe\xb8\x02\x1a\x02\x08\x01\x12\x1b\n\x15INPUT_INVALID_REQUEST\x10\xbf\xb8\x02\x12\x1d\n\x17PREDICT_INVALID_REQUEST\x10\xc1\xb8\x02\x12\x1c\n\x16SEARCH_INVALID_REQUEST\x10\xc2\xb8\x02\x12\x1e\n\x18\x43ONCEPTS_INVALID_REQUEST\x10\xc3\xb8\x02\x12\x1b\n\x15STATS_INVALID_REQUEST\x10\xc4\xb8\x02\x12\x1c\n\x16\x44\x41TABASE_DUPLICATE_KEY\x10\xca\xb8\x02\x12 \n\x1a\x44\x41TABASE_STATEMENT_TIMEOUT\x10\xcb\xb8\x02\x12$\n\x1e\x44\x41TABASE_INVALID_ROWS_AFFECTED\x10\xcc\xb8\x02\x12 \n\x1a\x44\x41TABASE_DEADLOCK_DETECTED\x10\xcd\xb8\x02\x12\x18\n\x12\x44\x41TABASE_FAIL_TASK\x10\xce\xb8\x02\x12&\n DATABASE_FAIL_TO_GET_CONNECTIONS\x10\xcf\xb8\x02\x12\x1f\n\x19\x44\x41TABASE_TOO_MANY_CLIENTS\x10\xd0\xb8\x02\x12\"\n\x1c\x44\x41TABASE_CONSTRAINT_VIOLATED\x10\xd1\xb8\x02\x12\x17\n\x11\x44\x41TABASE_CANCELED\x10\xd5\xb8\x02\x12\x1f\n\x19\x41SYNC_WORKER_MULTI_ERRORS\x10\xd4\xb8\x02\x12\x1c\n\x16RPC_REQUEST_QUEUE_FULL\x10\xde\xb8\x02\x12\x1c\n\x16RPC_SERVER_UNAVAILABLE\x10\xdf\xb8\x02\x12\x19\n\x13RPC_REQUEST_TIMEOUT\x10\xe0\xb8\x02\x12#\n\x1dRPC_MAX_MESSAGE_SIZE_EXCEEDED\x10\xe1\xb8\x02\x12\x12\n\x0cRPC_CANCELED\x10\xe3\xb8\x02\x12\x18\n\x12RPC_UNKNOWN_METHOD\x10\xe4\xb8\x02\x12\x1e\n\x18REQUEST_CANCELED_BY_USER\x10\xe5\xb8\x02\x12\x1e\n\x18\x43LUSTER_INTERNAL_FAILURE\x10\xa0\xd0\x02\x12\x1f\n\x19\x45XTERNAL_CONNECTION_ERROR\x10\xe2\xb8\x02\x12\x1a\n\x14QUERY_INVALID_SYNTAX\x10\xf2\xb8\x02\x12\x16\n\x10QUEUE_CONN_ERROR\x10\xa8\xc0\x02\x12!\n\x1bQUEUE_CLOSE_REQUEST_TIMEOUT\x10\xaa\xc0\x02\x12\x17\n\x11QUEUE_CONN_CLOSED\x10\xab\xc0\x02\x12\x1f\n\x19QUEUE_PUBLISH_ACK_TIMEOUT\x10\xac\xc0\x02\x12\x19\n\x13QUEUE_PUBLISH_ERROR\x10\xad\xc0\x02\x12 \n\x1aQUEUE_SUBSCRIPTION_TIMEOUT\x10\xae\xc0\x02\x12\x1e\n\x18QUEUE_SUBSCRIPTION_ERROR\x10\xaf\xc0\x02\x12\x1e\n\x18QUEUE_MARSHALLING_FAILED\x10\xb0\xc0\x02\x12 \n\x1aQUEUE_UNMARSHALLING_FAILED\x10\xb1\xc0\x02\x12\'\n!QUEUE_MAX_MSG_REDELIVERY_EXCEEDED\x10\xb2\xc0\x02\x12\x17\n\x11QUEUE_ACK_FAILURE\x10\xb3\xc0\x02\x12\x13\n\rSQS_OVERLIMIT\x10\x8c\xc1\x02\x12 \n\x1aSQS_INVALID_RECEIPT_HANDLE\x10\x8d\xc1\x02\x12\x11\n\x0bSQS_UNKNOWN\x10\x8e\xc1\x02\x12\x1d\n\x17SEARCH_INTERNAL_FAILURE\x10\xf9\xcf\x02\x12\x1f\n\x19SEARCH_PROJECTION_FAILURE\x10\xfa\xcf\x02\x12\x1f\n\x19SEARCH_PREDICTION_FAILURE\x10\xfb\xcf\x02\x12\'\n!SEARCH_BY_NOT_FULLY_INDEXED_INPUT\x10\xfc\xcf\x02\x12 \n\x1aSAVED_SEARCH_MODIFY_FAILED\x10\xfd\xcf\x02\x12\x1f\n\x19SEARCH_COUNTS_UNAVAILABLE\x10\xfe\xcf\x02\x12\x17\n\x11\x45VALUATION_QUEUED\x10\xdc\xd0\x02\x12\x1c\n\x16\x45VALUATION_IN_PROGRESS\x10\xdd\xd0\x02\x12\x18\n\x12\x45VALUATION_SUCCESS\x10\xde\xd0\x02\x12(\n\"EVALUATION_FAILED_TO_RETRIEVE_DATA\x10\xdf\xd0\x02\x12!\n\x1b\x45VALUATION_INVALID_ARGUMENT\x10\xe0\xd0\x02\x12\x17\n\x11\x45VALUATION_FAILED\x10\xe1\xd0\x02\x12\x18\n\x12\x45VALUATION_PENDING\x10\xe2\xd0\x02\x12\x1a\n\x14\x45VALUATION_TIMED_OUT\x10\xe3\xd0\x02\x12!\n\x1b\x45VALUATION_UNEXPECTED_ERROR\x10\xe4\xd0\x02\x12\x16\n\x10\x45VALUATION_MIXED\x10\xe5\xd0\x02\x12\x18\n\x12STRIPE_EVENT_ERROR\x10\xe1\xd7\x02\x12\x10\n\nCACHE_MISS\x10\xc9\xdf\x02\x12&\n REDIS_SCRIPT_EXITED_WITH_FAILURE\x10\xca\xdf\x02\x12\x16\n\x10REDIS_STREAM_ERR\x10\xcb\xdf\x02\x12\x18\n\x12REDIS_NO_CONSUMERS\x10\xcc\xdf\x02\x12\x1a\n\x14REDIS_STREAM_BACKOFF\x10\xcd\xdf\x02\x12\x18\n\x12SIGNUP_EVENT_ERROR\x10\xb1\xe7\x02\x12\x14\n\x0eSIGNUP_FLAGGED\x10\xb2\xe7\x02\x12\x1a\n\x14\x46ILETYPE_UNSUPPORTED\x10\xb3\xe7\x02\x12\x1f\n\x19\x41PP_COUNT_INVALID_MESSAGE\x10\x99\xef\x02\x12\'\n!APP_COUNT_UPDATE_INCREMENT_FAILED\x10\x9a\xef\x02\x12\x1e\n\x18\x41PP_COUNT_REBUILD_FAILED\x10\x9b\xef\x02\x12 \n\x1a\x41PP_COUNT_INTERNAL_FAILURE\x10\x9c\xef\x02\x12\x17\n\x11MP_DOWNLOAD_ERROR\x10\xfd\xef\x02\x12\x1a\n\x14MP_RESOLVE_DNS_ERROR\x10\xfe\xef\x02\x12)\n#MP_DOWNLOAD_MAX_SIZE_EXCEEDED_ERROR\x10\xff\xef\x02\x12\x1b\n\x15MP_IMAGE_DECODE_ERROR\x10\x80\xf0\x02\x12\x19\n\x13MP_INVALID_ARGUMENT\x10\x81\xf0\x02\x12\x1f\n\x19MP_IMAGE_PROCESSING_ERROR\x10\x82\xf0\x02\x12\x19\n\x13\x44\x41TATIER_CONN_ERROR\x10\xe1\xf0\x02\x12\x17\n\x11USER_CONSENT_FACE\x10\xd1\x86\x03\x12\x14\n\x0eWORKER_MISSING\x10\xb8\x8e\x03\x12\x13\n\rWORKER_ACTIVE\x10\xb9\x8e\x03\x12\x15\n\x0fWORKER_INACTIVE\x10\xba\x8e\x03\x12\x17\n\x11\x43OLLECTOR_MISSING\x10\xa0\x96\x03\x12\x16\n\x10\x43OLLECTOR_ACTIVE\x10\xa1\x96\x03\x12\x18\n\x12\x43OLLECTOR_INACTIVE\x10\xa2\x96\x03\x12!\n\x1b\x43OLLECTOR_POST_INPUT_FAILED\x10\xa3\x96\x03\x12*\n$SSO_IDENTITY_PROVIDER_DOES_NOT_EXIST\x10\x89\x9e\x03\x12\x16\n\x10TASK_IN_PROGRESS\x10\xf1\xa5\x03\x12\x0f\n\tTASK_DONE\x10\xf2\xa5\x03\x12\x12\n\x0cTASK_WONT_DO\x10\xf3\xa5\x03\x12\"\n\x1cTASK_ADD_ANNOTATIONS_FAILURE\x10\xf5\xa5\x03\x12\x13\n\rTASK_CONFLICT\x10\xd4\xa6\x03\x12\x1a\n\x14TASK_NOT_IMPLEMENTED\x10\xd5\xa6\x03\x12\x12\n\x0cTASK_MISSING\x10\xd6\xa6\x03\x12\x19\n\x13LABEL_ORDER_PENDING\x10\xd9\xad\x03\x12\x1d\n\x17LABEL_ORDER_IN_PROGRESS\x10\xda\xad\x03\x12\x19\n\x13LABEL_ORDER_SUCCESS\x10\xdb\xad\x03\x12\x1a\n\x14LABEL_ORDER_CANCELED\x10\xdc\xad\x03\x12\x14\n\x0eLICENSE_ACTIVE\x10\xe0\xd4\x03\x12\x1c\n\x16LICENSE_DOES_NOT_EXIST\x10\xe1\xd4\x03\x12\x19\n\x13LICENSE_NEED_UPDATE\x10\xe2\xd4\x03\x12\x15\n\x0fLICENSE_EXPIRED\x10\xe3\xd4\x03\x12\x15\n\x0fLICENSE_REVOKED\x10\xe4\xd4\x03\x12\x15\n\x0fLICENSE_DELETED\x10\xe5\xd4\x03\x12\x1d\n\x17LICENSE_VOLUME_EXCEEDED\x10\xe6\xd4\x03\x12!\n\x1bPASSWORD_VALIDATION_SUCCESS\x10\xc8\xdc\x03\x12 \n\x1aPASSWORD_VALIDATION_FAILED\x10\xc9\xdc\x03\x12%\n\x1fPASSWORDPOLICY_INVALID_ARGUMENT\x10\xca\xdc\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_CONFIG_NOT_FOUND\x10\xb0\xe4\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_INVALID_ARGUMENT\x10\xb1\xe4\x03\x12\x19\n\x13\x46\x45\x41TUREFLAG_BLOCKED\x10\xb2\xe4\x03\x12\x19\n\x13MAINTENANCE_SUCCESS\x10\x98\xec\x03\x12\x18\n\x12MAINTENANCE_FAILED\x10\x99\xec\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_PENDING\x10\x85\xf4\x03\x12!\n\x1b\x44\x41TASET_VERSION_IN_PROGRESS\x10\x8a\xf4\x03\x12\x1b\n\x15\x44\x41TASET_VERSION_READY\x10\x8f\xf4\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_FAILURE\x10\x94\xf4\x03\x12&\n DATASET_VERSION_UNEXPECTED_ERROR\x10\x99\xf4\x03\x12\x1e\n\x18\x44\x41TASET_VERSION_CONFLICT\x10\x9e\xf4\x03\x12\x1b\n\x15\x44\x41TASET_INPUT_SUCCESS\x10\xe4\xf4\x03\x12\x1d\n\x17\x44\x41TASET_INPUT_DUPLICATE\x10\xe5\xf4\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_SUCCESS\x10\xc8\xf5\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_PENDING\x10\xc9\xf5\x03\x12#\n\x1d\x44\x41TASET_VERSION_EXPORT_FAILED\x10\xca\xf5\x03\x12(\n\"DATASET_VERSION_EXPORT_IN_PROGRESS\x10\xcb\xf5\x03\x12-\n\'DATASET_VERSION_EXPORT_UNEXPECTED_ERROR\x10\xcc\xf5\x03\x12\x10\n\nJOB_QUEUED\x10\x80\xf4\x03\x12\x11\n\x0bJOB_RUNNING\x10\x81\xf4\x03\x12\x13\n\rJOB_COMPLETED\x10\x82\xf4\x03\x12\x10\n\nJOB_FAILED\x10\x83\xf4\x03\x12\x13\n\rJOB_CANCELLED\x10\x84\xf4\x03\x12\x1a\n\x14JOB_UNEXPECTED_ERROR\x10\x86\xf4\x03\x12\x12\n\x0cJOB_CONFLICT\x10\x87\xf4\x03\x12\x1c\n\x16\x41UTH_MISSING_IDP_ASSOC\x10\xe8\xfb\x03\x12\x19\n\x13LIST_OBJECTS_FAILED\x10\xd0\x83\x04\x12\x1c\n\x16\x41RCHIVE_EXTRACT_FAILED\x10\xb8\x8b\x04\x12\x18\n\x12UPLOAD_IN_PROGRESS\x10\xa0\x93\x04\x12\x11\n\x0bUPLOAD_DONE\x10\xa1\x93\x04\x12\x13\n\rUPLOAD_FAILED\x10\xa2\x93\x04\x12\x1d\n\x17UPLOAD_UNEXPECTED_ERROR\x10\xa3\x93\x04\x12\x14\n\x0eUPLOAD_EXPIRED\x10\xa4\x93\x04\x12\x15\n\x0fUPLOAD_CANCELED\x10\xa5\x93\x04\x12\x15\n\x0fUPLOAD_CONFLICT\x10\xa6\x93\x04\x12\x1a\n\x14\x42ILLING_INVALID_INFO\x10\x88\x9b\x04\x12\x1b\n\x15INTERNAL_SERVER_ISSUE\x10\xd4\xfd\x05\x12\x1d\n\x17INTERNAL_FETCHING_ISSUE\x10\xd5\xfd\x05\x12\x1d\n\x17INTERNAL_DATABASE_ISSUE\x10\xd6\xfd\x05\x12!\n\x1bINTERNAL_UNEXPECTED_TIMEOUT\x10\xd9\xfd\x05\x12\x1c\n\x16INTERNAL_UNEXPECTED_V1\x10\xda\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_PANIC\x10\xdb\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_SPIRE\x10\xdc\xfd\x05\x12 \n\x1aINTERNAL_REDIS_UNAVAILABLE\x10\xdd\xfd\x05\x12!\n\x1bINTERNAL_RESOURCE_EXHAUSTED\x10\xde\xfd\x05\x12\"\n\x1cINTERNAL_REDIS_UNCATEGORIZED\x10\xdf\xfd\x05\x12 \n\x1aINTERNAL_AWS_UNCATEGORIZED\x10\xe0\xfd\x05\x12\"\n\x1cINTERNAL_AZURE_UNCATEGORIZED\x10\xe1\xfd\x05\x12\x18\n\x12\x43ONN_UNCATEGORIZED\x10\xb9\x85\x06\x12\x19\n\x13MODEL_UNCATEGORIZED\x10\xba\x85\x06\x12\x19\n\x13INPUT_UNCATEGORIZED\x10\xbb\x85\x06\x12\x1e\n\x18\x41NNOTATION_UNCATEGORIZED\x10\xbc\x85\x06\x12\x1b\n\x15\x42ILLING_UNCATEGORIZED\x10\xbd\x85\x06\x12\x1c\n\x16INTERNAL_UNCATEGORIZED\x10\xc1\x85\x06\x12\x11\n\x0b\x42\x41\x44_REQUEST\x10\xa0\xc2\x05\x12\x12\n\x0cSERVER_ERROR\x10\x84\xc3\x05\"\x08\x08\xbf\xc6\x01\x10\xbf\xc6\x01\"\x08\x08\xe8\x81\x02\x10\xe8\x81\x02\"\x08\x08\xe9\x81\x02\x10\xe9\x81\x02\"\x08\x08\xea\x81\x02\x10\xea\x81\x02\"\x08\x08\xcc\x82\x02\x10\xcc\x82\x02\"\x08\x08\xcd\x82\x02\x10\xcd\x82\x02\"\x08\x08\xce\x82\x02\x10\xce\x82\x02\"\x08\x08\xcf\x82\x02\x10\xcf\x82\x02\"\x08\x08\xd0\x82\x02\x10\xd0\x82\x02\"\x08\x08\xd1\x82\x02\x10\xd1\x82\x02\"\x08\x08\xd2\x82\x02\x10\xd2\x82\x02\"\x08\x08\xb0\x83\x02\x10\xb0\x83\x02\"\x08\x08\xb1\x83\x02\x10\xb1\x83\x02\"\x08\x08\xb3\x83\x02\x10\xb3\x83\x02\"\x08\x08\xba\x83\x02\x10\xba\x83\x02\"\x08\x08\xbb\xb8\x02\x10\xbb\xb8\x02\"\x08\x08\xd2\xb8\x02\x10\xd2\xb8\x02\"\x08\x08\xd3\xb8\x02\x10\xd3\xb8\x02\"\x08\x08\xf0\xc1\x02\x10\xf0\xc1\x02\"\x08\x08\xf1\xc1\x02\x10\xf1\xc1\x02\"\x08\x08\xf2\xc1\x02\x10\xf2\xc1\x02\"\x08\x08\xf3\xc1\x02\x10\xf3\xc1\x02\"\x08\x08\xf4\xc1\x02\x10\xf4\xc1\x02\"\x08\x08\x9c\xc7\x01\x10\x9c\xc7\x01\"\x08\x08\x9d\xc7\x01\x10\x9d\xc7\x01\"\x08\x08\x9e\xc7\x01\x10\x9e\xc7\x01\"\x08\x08\x9f\xc7\x01\x10\x9f\xc7\x01\"\x08\x08\xa1\xc7\x01\x10\xa1\xc7\x01\"\x08\x08\xa2\xc7\x01\x10\xa2\xc7\x01\x42g\n\x1c\x63om.clarifai.grpc.api.statusP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+proto/clarifai/api/status/status_code.proto\x12\x13\x63larifai.api.status*\xe0T\n\nStatusCode\x12\x08\n\x04ZERO\x10\x00\x12\x0c\n\x07SUCCESS\x10\x90N\x12\x11\n\x0cMIXED_STATUS\x10\x9aN\x12\x0c\n\x07\x46\x41ILURE\x10\xa4N\x12\x0e\n\tTRY_AGAIN\x10\xaeN\x12\x14\n\x0fNOT_IMPLEMENTED\x10\xb8N\x12\n\n\x05MOVED\x10\xc2N\x12\x18\n\x13\x43ONN_ACCOUNT_ISSUES\x10\xf8U\x12\x1b\n\x12\x43ONN_TOKEN_INVALID\x10\xf9U\x1a\x02\x08\x01\x12\x1d\n\x18\x43ONN_CREDENTIALS_INVALID\x10\xfaU\x12\x1d\n\x18\x43ONN_EXCEED_HOURLY_LIMIT\x10\xfbU\x12\x1e\n\x19\x43ONN_EXCEED_MONTHLY_LIMIT\x10\xfcU\x12\x13\n\x0e\x43ONN_THROTTLED\x10\xfdU\x12\x18\n\x13\x43ONN_EXCEEDS_LIMITS\x10\xfeU\x12\x1d\n\x18\x43ONN_INSUFFICIENT_SCOPES\x10\xffU\x12\x15\n\x10\x43ONN_KEY_INVALID\x10\x80V\x12\x17\n\x12\x43ONN_KEY_NOT_FOUND\x10\x81V\x12\x1c\n\x17\x43ONN_BAD_REQUEST_FORMAT\x10\xdcV\x12\x18\n\x13\x43ONN_DOES_NOT_EXIST\x10\xddV\x12\x19\n\x14\x43ONN_INVALID_REQUEST\x10\xdeV\x12\x1c\n\x17\x43ONN_METHOD_NOT_ALLOWED\x10\xdfV\x12\x19\n\x14\x43ONN_NO_GDPR_CONSENT\x10\xe0V\x12\x1e\n\x19\x43ONN_AUTH_METHOD_DISABLED\x10\xc0W\x12\x13\n\rMODEL_TRAINED\x10\xec\xa4\x01\x12\x14\n\x0eMODEL_TRAINING\x10\xed\xa4\x01\x12\x15\n\x0fMODEL_UNTRAINED\x10\xee\xa4\x01\x12\x1f\n\x19MODEL_QUEUED_FOR_TRAINING\x10\xef\xa4\x01\x12\x15\n\x0fMODEL_UPLOADING\x10\xf0\xa4\x01\x12\x1c\n\x16MODEL_UPLOADING_FAILED\x10\xf1\xa4\x01\x12\x1b\n\x15MODEL_TRAINING_FAILED\x10\xf2\xa4\x01\x12\x1c\n\x16MODEL_TRAINING_NO_DATA\x10\xf6\xa4\x01\x12!\n\x1bMODEL_TRAINING_NO_POSITIVES\x10\xf7\xa4\x01\x12*\n$MODEL_TRAINING_ONE_VS_N_SINGLE_CLASS\x10\xf8\xa4\x01\x12\x1e\n\x18MODEL_TRAINING_TIMED_OUT\x10\xf9\xa4\x01\x12\"\n\x1cMODEL_TRAINING_WAITING_ERROR\x10\xfa\xa4\x01\x12\"\n\x1cMODEL_TRAINING_UNKNOWN_ERROR\x10\xfb\xa4\x01\x12&\n\x1cMODEL_TRAINING_MSG_REDELIVER\x10\xfc\xa4\x01\x1a\x02\x08\x01\x12&\n MODEL_TRAINING_INSUFFICIENT_DATA\x10\xfd\xa4\x01\x12#\n\x1dMODEL_TRAINING_INVALID_PARAMS\x10\xfe\xa4\x01\x12\x34\n.MODEL_TRAINING_INVALID_DATA_TOLERANCE_EXCEEDED\x10\xff\xa4\x01\x12\x1a\n\x14MODEL_MODIFY_SUCCESS\x10\x9e\xa5\x01\x12\x1a\n\x14MODEL_MODIFY_PENDING\x10\x9f\xa5\x01\x12\x19\n\x13MODEL_MODIFY_FAILED\x10\xa0\xa5\x01\x12\x1a\n\x14MODEL_DOES_NOT_EXIST\x10\xd0\xa5\x01\x12\x1d\n\x17MODEL_PERMISSION_DENIED\x10\xd1\xa5\x01\x12\x1c\n\x16MODEL_INVALID_ARGUMENT\x10\xd2\xa5\x01\x12\x1b\n\x15MODEL_INVALID_REQUEST\x10\xd3\xa5\x01\x12\x15\n\x0fMODEL_EVALUATED\x10\xb4\xa6\x01\x12\x16\n\x10MODEL_EVALUATING\x10\xb5\xa6\x01\x12\x19\n\x13MODEL_NOT_EVALUATED\x10\xb6\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_EVALUATION\x10\xb7\xa6\x01\x12 \n\x1aMODEL_EVALUATION_TIMED_OUT\x10\xbe\xa6\x01\x12$\n\x1eMODEL_EVALUATION_WAITING_ERROR\x10\xbf\xa6\x01\x12$\n\x1eMODEL_EVALUATION_UNKNOWN_ERROR\x10\xc0\xa6\x01\x12\x1d\n\x17MODEL_PREDICTION_FAILED\x10\xc1\xa6\x01\x12(\n\x1eMODEL_EVALUATION_MSG_REDELIVER\x10\xc2\xa6\x01\x1a\x02\x08\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_LABELS\x10\xc3\xa6\x01\x12\"\n\x1cMODEL_EVALUATION_NEED_INPUTS\x10\xc4\xa6\x01\x12\x1d\n\x17MODEL_EVALUATION_FAILED\x10\xc5\xa6\x01\x12\x1d\n\x17MODEL_DEPLOYMENT_FAILED\x10\xe6\xa6\x01\x12\x15\n\x0fMODEL_DEPLOYING\x10\xe7\xa6\x01\x12!\n\x1bMODEL_QUEUED_FOR_DEPLOYMENT\x10\xe8\xa6\x01\x12\x18\n\x12MODEL_NOT_DEPLOYED\x10\xe9\xa6\x01\x12&\n MODEL_REFERENCE_INVALID_ARGUMENT\x10\x98\xa7\x01\x12*\n$MODEL_EXAMPLE_INPUT_INVALID_ARGUMENT\x10\xac\xa7\x01\x12 \n\x1aWORKFLOW_NO_MATCHING_INPUT\x10\xf1\xab\x01\x12$\n\x1eWORKFLOW_REQUIRE_TRAINED_MODEL\x10\xf2\xab\x01\x12\x18\n\x12WORKFLOW_DUPLICATE\x10\xd4\xac\x01\x12!\n\x1bWORKFLOW_UNSUPPORTED_FORMAT\x10\xd5\xac\x01\x12\x1d\n\x17WORKFLOW_DOES_NOT_EXIST\x10\xd6\xac\x01\x12 \n\x1aWORKFLOW_PERMISSION_DENIED\x10\xd7\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_ARGUMENT\x10\xd8\xac\x01\x12\x1d\n\x17WORKFLOW_INVALID_RECIPE\x10\xd9\xac\x01\x12\x1f\n\x19WORKFLOW_INVALID_TEMPLATE\x10\xda\xac\x01\x12\x1c\n\x16WORKFLOW_INVALID_GRAPH\x10\xdb\xac\x01\x12\x1f\n\x19WORKFLOW_INTERNAL_FAILURE\x10\xdc\xac\x01\x12\x1e\n\x18WORKFLOW_INVALID_REQUEST\x10\xd7\xb3\x01\x12\x1d\n\x17WORKFLOW_MODIFY_SUCCESS\x10\x86\xad\x01\x12\x1d\n\x17WORKFLOW_MODIFY_PENDING\x10\x87\xad\x01\x12\x1c\n\x16WORKFLOW_MODIFY_FAILED\x10\x88\xad\x01\x12\x1d\n\x17WORKFLOW_REINDEX_FAILED\x10\x89\xad\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_SUCCESS\x10\xee\xb4\x01\x12\x1c\n\x16\x43ONCEPT_MODIFY_PENDING\x10\xef\xb4\x01\x12\x1b\n\x15\x43ONCEPT_MODIFY_FAILED\x10\xf0\xb4\x01\x12\x18\n\x12\x41NNOTATION_SUCCESS\x10\xd6\xbc\x01\x12\x18\n\x12\x41NNOTATION_PENDING\x10\xd7\xbc\x01\x12\x17\n\x11\x41NNOTATION_FAILED\x10\xd8\xbc\x01\x12\x1f\n\x19\x41NNOTATION_UNKNOWN_STATUS\x10\xda\xbc\x01\x12!\n\x1b\x41NNOTATION_INVALID_ARGUMENT\x10\xdb\xbc\x01\x12\"\n\x1c\x41NNOTATION_PERMISSION_DENIED\x10\xdc\xbc\x01\x12 \n\x1a\x41NNOTATION_AWAITING_REVIEW\x10\xdd\xbc\x01\x12*\n$ANNOTATION_AWAITING_CONSENSUS_REVIEW\x10\xdf\xbc\x01\x12\x1e\n\x18\x41NNOTATION_REVIEW_DENIED\x10\xde\xbc\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_SUCCESS\x10\xba\xbd\x01\x12\x1f\n\x19\x41NNOTATION_MODIFY_PENDING\x10\xbb\xbd\x01\x12\x1e\n\x18\x41NNOTATION_MODIFY_FAILED\x10\xbc\xbd\x01\x12&\n METADATA_INVALID_PATCH_ARGUMENTS\x10\xc4\xc2\x01\x12\x1c\n\x16METADATA_PARSING_ISSUE\x10\xc5\xc2\x01\x12!\n\x1bMETADATA_MANIPULATION_ISSUE\x10\xc6\xc2\x01\x12\x1c\n\x16TRAINER_JOB_STATE_NONE\x10\xa8\xc3\x01\x12\x1e\n\x18TRAINER_JOB_STATE_QUEUED\x10\xa9\xc3\x01\x12\x1f\n\x19TRAINER_JOB_STATE_RUNNING\x10\xaa\xc3\x01\x12 \n\x1aTRAINER_JOB_STATE_COMPLETE\x10\xab\xc3\x01\x12\x1d\n\x17TRAINER_JOB_STATE_ERROR\x10\xac\xc3\x01\x12\x17\n\x11\x44\x41TA_DUMP_SUCCESS\x10\xbe\xc4\x01\x12\x17\n\x11\x44\x41TA_DUMP_PENDING\x10\xbf\xc4\x01\x12\x16\n\x10\x44\x41TA_DUMP_FAILED\x10\xc0\xc4\x01\x12\x1b\n\x15\x44\x41TA_DUMP_IN_PROGRESS\x10\xc1\xc4\x01\x12\x1b\n\x11\x44\x41TA_DUMP_NO_DATA\x10\xc2\xc4\x01\x1a\x02\x08\x01\x12 \n\x1a\x44\x41TA_DUMP_UNEXPECTED_ERROR\x10\xc3\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_SUCCESS\x10\xd2\xc4\x01\x12\x1e\n\x18\x44\x41TA_DUMP_EXPORT_PENDING\x10\xd3\xc4\x01\x12\x1d\n\x17\x44\x41TA_DUMP_EXPORT_FAILED\x10\xd4\xc4\x01\x12\"\n\x1c\x44\x41TA_DUMP_EXPORT_IN_PROGRESS\x10\xd5\xc4\x01\x12\'\n!DATA_DUMP_EXPORT_UNEXPECTED_ERROR\x10\xd6\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_SUCCESS\x10\xf0\xc4\x01\x12\x1c\n\x16\x41PP_DUPLICATION_FAILED\x10\xf1\xc4\x01\x12\x1d\n\x17\x41PP_DUPLICATION_PENDING\x10\xf2\xc4\x01\x12!\n\x1b\x41PP_DUPLICATION_IN_PROGRESS\x10\xf3\xc4\x01\x12%\n\x1f\x41PP_DUPLICATION_INVALID_REQUEST\x10\xf4\xc4\x01\x12\x1b\n\x15MODULE_DOES_NOT_EXIST\x10\xd4\xc5\x01\x12\x1e\n\x18MODULE_PERMISSION_DENIED\x10\xd5\xc5\x01\x12\x1d\n\x17MODULE_INVALID_ARGUMENT\x10\xd6\xc5\x01\x12\x1c\n\x16MODULE_INVALID_REQUEST\x10\xd7\xc5\x01\x12\x1c\n\x16\x42ULK_OPERATION_SUCCESS\x10\xb8\xc6\x01\x12\x1b\n\x15\x42ULK_OPERATION_FAILED\x10\xb9\xc6\x01\x12\x1c\n\x16\x42ULK_OPERATION_PENDING\x10\xba\xc6\x01\x12 \n\x1a\x42ULK_OPERATION_IN_PROGRESS\x10\xbb\xc6\x01\x12$\n\x1e\x42ULK_OPERATION_INVALID_REQUEST\x10\xbc\xc6\x01\x12\x1e\n\x18\x42ULK_OPERATION_CANCELLED\x10\xbd\xc6\x01\x12%\n\x1f\x42ULK_OPERATION_UNEXPECTED_ERROR\x10\xbe\xc6\x01\x12\x1b\n\x15RUNNER_DOES_NOT_EXIST\x10\x80\xc8\x01\x12\x1e\n\x18RUNNER_PERMISSION_DENIED\x10\x81\xc8\x01\x12\x1d\n\x17RUNNER_INVALID_ARGUMENT\x10\x82\xc8\x01\x12\x1c\n\x16RUNNER_INVALID_REQUEST\x10\x83\xc8\x01\x12\x18\n\x12RUNNER_NEEDS_RETRY\x10\x84\xc8\x01\x12\x1c\n\x16INPUT_DOWNLOAD_SUCCESS\x10\xb0\xea\x01\x12\x1c\n\x16INPUT_DOWNLOAD_PENDING\x10\xb1\xea\x01\x12\x1b\n\x15INPUT_DOWNLOAD_FAILED\x10\xb2\xea\x01\x12 \n\x1aINPUT_DOWNLOAD_IN_PROGRESS\x10\xb3\xea\x01\x12 \n\x1aINPUT_STATUS_UPDATE_FAILED\x10\xb4\xea\x01\x12\x19\n\x13INPUT_DELETE_FAILED\x10\xb5\xea\x01\x12\x15\n\x0fINPUT_DUPLICATE\x10\x94\xeb\x01\x12\x1e\n\x18INPUT_UNSUPPORTED_FORMAT\x10\x95\xeb\x01\x12\x1a\n\x14INPUT_DOES_NOT_EXIST\x10\x96\xeb\x01\x12\x1d\n\x17INPUT_PERMISSION_DENIED\x10\x97\xeb\x01\x12\x1c\n\x16INPUT_INVALID_ARGUMENT\x10\x98\xeb\x01\x12\x16\n\x10INPUT_OVER_LIMIT\x10\x99\xeb\x01\x12\x17\n\x11INPUT_INVALID_URL\x10\x9a\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_SUCCESS\x10\xf8\xeb\x01\x12\x1a\n\x14INPUT_MODIFY_PENDING\x10\xf9\xeb\x01\x12\x19\n\x13INPUT_MODIFY_FAILED\x10\xfb\xeb\x01\x12\x1f\n\x19INPUT_STORAGE_HOST_FAILED\x10\x82\xec\x01\x12\x1d\n\x17\x41LL_INPUT_INVALID_BYTES\x10\xdc\xec\x01\x12\x1b\n\x15INPUT_CLUSTER_SUCCESS\x10\xc0\xed\x01\x12\x1b\n\x15INPUT_CLUSTER_PENDING\x10\xc1\xed\x01\x12\x1a\n\x14INPUT_CLUSTER_FAILED\x10\xc2\xed\x01\x12\x1f\n\x19INPUT_CLUSTER_IN_PROGRESS\x10\xc3\xed\x01\x12\x1b\n\x15INPUT_REINDEX_SUCCESS\x10\xa4\xee\x01\x12\x1b\n\x15INPUT_REINDEX_PENDING\x10\xa5\xee\x01\x12\x1a\n\x14INPUT_REINDEX_FAILED\x10\xa6\xee\x01\x12\x1f\n\x19INPUT_REINDEX_IN_PROGRESS\x10\xa7\xee\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_SUCCESS\x10\x98\xf2\x01\x12\"\n\x1cINPUT_VIDEO_DOWNLOAD_PENDING\x10\x99\xf2\x01\x12!\n\x1bINPUT_VIDEO_DOWNLOAD_FAILED\x10\x9a\xf2\x01\x12\x1b\n\x15INPUT_VIDEO_DUPLICATE\x10\xfc\xf2\x01\x12$\n\x1eINPUT_VIDEO_UNSUPPORTED_FORMAT\x10\xfd\xf2\x01\x12 \n\x1aINPUT_VIDEO_DOES_NOT_EXIST\x10\xfe\xf2\x01\x12#\n\x1dINPUT_VIDEO_PERMISSION_DENIED\x10\xff\xf2\x01\x12\"\n\x1cINPUT_VIDEO_INVALID_ARGUMENT\x10\x80\xf3\x01\x12\x1c\n\x16INPUT_VIDEO_OVER_LIMIT\x10\x81\xf3\x01\x12\x1d\n\x17INPUT_VIDEO_INVALID_URL\x10\x82\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_SUCCESS\x10\xe0\xf3\x01\x12 \n\x1aINPUT_VIDEO_MODIFY_PENDING\x10\xe1\xf3\x01\x12\x1f\n\x19INPUT_VIDEO_MODIFY_FAILED\x10\xe3\xf3\x01\x12%\n\x1fINPUT_VIDEO_STORAGE_HOST_FAILED\x10\xea\xf3\x01\x12$\n\x1e\x41LL_INPUT_VIDEOS_INVALID_BYTES\x10\xc4\xf4\x01\x12$\n\x1eINPUT_VIDEO_PROCESSING_SUCCESS\x10\xa8\xf5\x01\x12$\n\x1eINPUT_VIDEO_PROCESSING_PENDING\x10\xb2\xf5\x01\x12#\n\x1dINPUT_VIDEO_PROCESSING_FAILED\x10\xbc\xf5\x01\x12\'\n!INPUT_VIDEO_STORAGE_INCONSISTENCY\x10\xc6\xf5\x01\x12!\n\x1bINPUT_VIDEO_STORAGE_FAILURE\x10\xd0\xf5\x01\x12(\n\"INPUT_VIDEO_URL_GENERATION_FAILURE\x10\xda\xf5\x01\x12\x1d\n\x17INPUT_CONNECTION_FAILED\x10\xbc\xb8\x02\x12&\n REQUEST_DISABLED_FOR_MAINTENANCE\x10\xbd\xb8\x02\x12/\n%INPUT_WRITES_DISABLED_FOR_MAINTENANCE\x10\xbe\xb8\x02\x1a\x02\x08\x01\x12\x1b\n\x15INPUT_INVALID_REQUEST\x10\xbf\xb8\x02\x12\x1d\n\x17PREDICT_INVALID_REQUEST\x10\xc1\xb8\x02\x12\x1c\n\x16SEARCH_INVALID_REQUEST\x10\xc2\xb8\x02\x12\x1e\n\x18\x43ONCEPTS_INVALID_REQUEST\x10\xc3\xb8\x02\x12\x1b\n\x15STATS_INVALID_REQUEST\x10\xc4\xb8\x02\x12\x1c\n\x16\x44\x41TABASE_DUPLICATE_KEY\x10\xca\xb8\x02\x12 \n\x1a\x44\x41TABASE_STATEMENT_TIMEOUT\x10\xcb\xb8\x02\x12$\n\x1e\x44\x41TABASE_INVALID_ROWS_AFFECTED\x10\xcc\xb8\x02\x12 \n\x1a\x44\x41TABASE_DEADLOCK_DETECTED\x10\xcd\xb8\x02\x12\x18\n\x12\x44\x41TABASE_FAIL_TASK\x10\xce\xb8\x02\x12&\n DATABASE_FAIL_TO_GET_CONNECTIONS\x10\xcf\xb8\x02\x12\x1f\n\x19\x44\x41TABASE_TOO_MANY_CLIENTS\x10\xd0\xb8\x02\x12\"\n\x1c\x44\x41TABASE_CONSTRAINT_VIOLATED\x10\xd1\xb8\x02\x12\x17\n\x11\x44\x41TABASE_CANCELED\x10\xd5\xb8\x02\x12\x1f\n\x19\x41SYNC_WORKER_MULTI_ERRORS\x10\xd4\xb8\x02\x12\x1c\n\x16RPC_REQUEST_QUEUE_FULL\x10\xde\xb8\x02\x12\x1c\n\x16RPC_SERVER_UNAVAILABLE\x10\xdf\xb8\x02\x12\x19\n\x13RPC_REQUEST_TIMEOUT\x10\xe0\xb8\x02\x12#\n\x1dRPC_MAX_MESSAGE_SIZE_EXCEEDED\x10\xe1\xb8\x02\x12\x12\n\x0cRPC_CANCELED\x10\xe3\xb8\x02\x12\x18\n\x12RPC_UNKNOWN_METHOD\x10\xe4\xb8\x02\x12\x1e\n\x18REQUEST_CANCELED_BY_USER\x10\xe5\xb8\x02\x12\x1e\n\x18\x43LUSTER_INTERNAL_FAILURE\x10\xa0\xd0\x02\x12\x1f\n\x19\x45XTERNAL_CONNECTION_ERROR\x10\xe2\xb8\x02\x12\x1a\n\x14QUERY_INVALID_SYNTAX\x10\xf2\xb8\x02\x12\x16\n\x10QUEUE_CONN_ERROR\x10\xa8\xc0\x02\x12!\n\x1bQUEUE_CLOSE_REQUEST_TIMEOUT\x10\xaa\xc0\x02\x12\x17\n\x11QUEUE_CONN_CLOSED\x10\xab\xc0\x02\x12\x1f\n\x19QUEUE_PUBLISH_ACK_TIMEOUT\x10\xac\xc0\x02\x12\x19\n\x13QUEUE_PUBLISH_ERROR\x10\xad\xc0\x02\x12 \n\x1aQUEUE_SUBSCRIPTION_TIMEOUT\x10\xae\xc0\x02\x12\x1e\n\x18QUEUE_SUBSCRIPTION_ERROR\x10\xaf\xc0\x02\x12\x1e\n\x18QUEUE_MARSHALLING_FAILED\x10\xb0\xc0\x02\x12 \n\x1aQUEUE_UNMARSHALLING_FAILED\x10\xb1\xc0\x02\x12\'\n!QUEUE_MAX_MSG_REDELIVERY_EXCEEDED\x10\xb2\xc0\x02\x12\x17\n\x11QUEUE_ACK_FAILURE\x10\xb3\xc0\x02\x12\x13\n\rSQS_OVERLIMIT\x10\x8c\xc1\x02\x12 \n\x1aSQS_INVALID_RECEIPT_HANDLE\x10\x8d\xc1\x02\x12\x11\n\x0bSQS_UNKNOWN\x10\x8e\xc1\x02\x12\x1d\n\x17SEARCH_INTERNAL_FAILURE\x10\xf9\xcf\x02\x12\x1f\n\x19SEARCH_PROJECTION_FAILURE\x10\xfa\xcf\x02\x12\x1f\n\x19SEARCH_PREDICTION_FAILURE\x10\xfb\xcf\x02\x12\'\n!SEARCH_BY_NOT_FULLY_INDEXED_INPUT\x10\xfc\xcf\x02\x12 \n\x1aSAVED_SEARCH_MODIFY_FAILED\x10\xfd\xcf\x02\x12\x1f\n\x19SEARCH_COUNTS_UNAVAILABLE\x10\xfe\xcf\x02\x12\x17\n\x11\x45VALUATION_QUEUED\x10\xdc\xd0\x02\x12\x1c\n\x16\x45VALUATION_IN_PROGRESS\x10\xdd\xd0\x02\x12\x18\n\x12\x45VALUATION_SUCCESS\x10\xde\xd0\x02\x12(\n\"EVALUATION_FAILED_TO_RETRIEVE_DATA\x10\xdf\xd0\x02\x12!\n\x1b\x45VALUATION_INVALID_ARGUMENT\x10\xe0\xd0\x02\x12\x17\n\x11\x45VALUATION_FAILED\x10\xe1\xd0\x02\x12\x18\n\x12\x45VALUATION_PENDING\x10\xe2\xd0\x02\x12\x1a\n\x14\x45VALUATION_TIMED_OUT\x10\xe3\xd0\x02\x12!\n\x1b\x45VALUATION_UNEXPECTED_ERROR\x10\xe4\xd0\x02\x12\x16\n\x10\x45VALUATION_MIXED\x10\xe5\xd0\x02\x12\x18\n\x12STRIPE_EVENT_ERROR\x10\xe1\xd7\x02\x12\x10\n\nCACHE_MISS\x10\xc9\xdf\x02\x12&\n REDIS_SCRIPT_EXITED_WITH_FAILURE\x10\xca\xdf\x02\x12\x16\n\x10REDIS_STREAM_ERR\x10\xcb\xdf\x02\x12\x18\n\x12REDIS_NO_CONSUMERS\x10\xcc\xdf\x02\x12\x1a\n\x14REDIS_STREAM_BACKOFF\x10\xcd\xdf\x02\x12\x18\n\x12SIGNUP_EVENT_ERROR\x10\xb1\xe7\x02\x12\x14\n\x0eSIGNUP_FLAGGED\x10\xb2\xe7\x02\x12\x1a\n\x14\x46ILETYPE_UNSUPPORTED\x10\xb3\xe7\x02\x12\x1f\n\x19\x41PP_COUNT_INVALID_MESSAGE\x10\x99\xef\x02\x12\'\n!APP_COUNT_UPDATE_INCREMENT_FAILED\x10\x9a\xef\x02\x12\x1e\n\x18\x41PP_COUNT_REBUILD_FAILED\x10\x9b\xef\x02\x12 \n\x1a\x41PP_COUNT_INTERNAL_FAILURE\x10\x9c\xef\x02\x12\x17\n\x11MP_DOWNLOAD_ERROR\x10\xfd\xef\x02\x12\x1a\n\x14MP_RESOLVE_DNS_ERROR\x10\xfe\xef\x02\x12)\n#MP_DOWNLOAD_MAX_SIZE_EXCEEDED_ERROR\x10\xff\xef\x02\x12\x1b\n\x15MP_IMAGE_DECODE_ERROR\x10\x80\xf0\x02\x12\x19\n\x13MP_INVALID_ARGUMENT\x10\x81\xf0\x02\x12\x1f\n\x19MP_IMAGE_PROCESSING_ERROR\x10\x82\xf0\x02\x12\x19\n\x13\x44\x41TATIER_CONN_ERROR\x10\xe1\xf0\x02\x12\x17\n\x11USER_CONSENT_FACE\x10\xd1\x86\x03\x12\x14\n\x0eWORKER_MISSING\x10\xb8\x8e\x03\x12\x13\n\rWORKER_ACTIVE\x10\xb9\x8e\x03\x12\x15\n\x0fWORKER_INACTIVE\x10\xba\x8e\x03\x12\x17\n\x11\x43OLLECTOR_MISSING\x10\xa0\x96\x03\x12\x16\n\x10\x43OLLECTOR_ACTIVE\x10\xa1\x96\x03\x12\x18\n\x12\x43OLLECTOR_INACTIVE\x10\xa2\x96\x03\x12!\n\x1b\x43OLLECTOR_POST_INPUT_FAILED\x10\xa3\x96\x03\x12*\n$SSO_IDENTITY_PROVIDER_DOES_NOT_EXIST\x10\x89\x9e\x03\x12\x16\n\x10TASK_IN_PROGRESS\x10\xf1\xa5\x03\x12\x0f\n\tTASK_DONE\x10\xf2\xa5\x03\x12\x12\n\x0cTASK_WONT_DO\x10\xf3\xa5\x03\x12\x11\n\x0bTASK_FAILED\x10\xf5\xa5\x03\x12\x0f\n\tTASK_IDLE\x10\xf6\xa5\x03\x12\x13\n\rTASK_CONFLICT\x10\xd4\xa6\x03\x12\x1a\n\x14TASK_NOT_IMPLEMENTED\x10\xd5\xa6\x03\x12\x12\n\x0cTASK_MISSING\x10\xd6\xa6\x03\x12\x19\n\x13LABEL_ORDER_PENDING\x10\xd9\xad\x03\x12\x1d\n\x17LABEL_ORDER_IN_PROGRESS\x10\xda\xad\x03\x12\x19\n\x13LABEL_ORDER_SUCCESS\x10\xdb\xad\x03\x12\x1a\n\x14LABEL_ORDER_CANCELED\x10\xdc\xad\x03\x12\x14\n\x0eLICENSE_ACTIVE\x10\xe0\xd4\x03\x12\x1c\n\x16LICENSE_DOES_NOT_EXIST\x10\xe1\xd4\x03\x12\x19\n\x13LICENSE_NEED_UPDATE\x10\xe2\xd4\x03\x12\x15\n\x0fLICENSE_EXPIRED\x10\xe3\xd4\x03\x12\x15\n\x0fLICENSE_REVOKED\x10\xe4\xd4\x03\x12\x15\n\x0fLICENSE_DELETED\x10\xe5\xd4\x03\x12\x1d\n\x17LICENSE_VOLUME_EXCEEDED\x10\xe6\xd4\x03\x12!\n\x1bPASSWORD_VALIDATION_SUCCESS\x10\xc8\xdc\x03\x12 \n\x1aPASSWORD_VALIDATION_FAILED\x10\xc9\xdc\x03\x12%\n\x1fPASSWORDPOLICY_INVALID_ARGUMENT\x10\xca\xdc\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_CONFIG_NOT_FOUND\x10\xb0\xe4\x03\x12\"\n\x1c\x46\x45\x41TUREFLAG_INVALID_ARGUMENT\x10\xb1\xe4\x03\x12\x19\n\x13\x46\x45\x41TUREFLAG_BLOCKED\x10\xb2\xe4\x03\x12\x19\n\x13MAINTENANCE_SUCCESS\x10\x98\xec\x03\x12\x18\n\x12MAINTENANCE_FAILED\x10\x99\xec\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_PENDING\x10\x85\xf4\x03\x12!\n\x1b\x44\x41TASET_VERSION_IN_PROGRESS\x10\x8a\xf4\x03\x12\x1b\n\x15\x44\x41TASET_VERSION_READY\x10\x8f\xf4\x03\x12\x1d\n\x17\x44\x41TASET_VERSION_FAILURE\x10\x94\xf4\x03\x12&\n DATASET_VERSION_UNEXPECTED_ERROR\x10\x99\xf4\x03\x12\x1e\n\x18\x44\x41TASET_VERSION_CONFLICT\x10\x9e\xf4\x03\x12\x1b\n\x15\x44\x41TASET_INPUT_SUCCESS\x10\xe4\xf4\x03\x12\x1d\n\x17\x44\x41TASET_INPUT_DUPLICATE\x10\xe5\xf4\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_SUCCESS\x10\xc8\xf5\x03\x12$\n\x1e\x44\x41TASET_VERSION_EXPORT_PENDING\x10\xc9\xf5\x03\x12#\n\x1d\x44\x41TASET_VERSION_EXPORT_FAILED\x10\xca\xf5\x03\x12(\n\"DATASET_VERSION_EXPORT_IN_PROGRESS\x10\xcb\xf5\x03\x12-\n\'DATASET_VERSION_EXPORT_UNEXPECTED_ERROR\x10\xcc\xf5\x03\x12\x10\n\nJOB_QUEUED\x10\x80\xf4\x03\x12\x11\n\x0bJOB_RUNNING\x10\x81\xf4\x03\x12\x13\n\rJOB_COMPLETED\x10\x82\xf4\x03\x12\x10\n\nJOB_FAILED\x10\x83\xf4\x03\x12\x13\n\rJOB_CANCELLED\x10\x84\xf4\x03\x12\x1a\n\x14JOB_UNEXPECTED_ERROR\x10\x86\xf4\x03\x12\x12\n\x0cJOB_CONFLICT\x10\x87\xf4\x03\x12\x1c\n\x16\x41UTH_MISSING_IDP_ASSOC\x10\xe8\xfb\x03\x12\x19\n\x13LIST_OBJECTS_FAILED\x10\xd0\x83\x04\x12\x1c\n\x16\x41RCHIVE_EXTRACT_FAILED\x10\xb8\x8b\x04\x12\x18\n\x12UPLOAD_IN_PROGRESS\x10\xa0\x93\x04\x12\x11\n\x0bUPLOAD_DONE\x10\xa1\x93\x04\x12\x13\n\rUPLOAD_FAILED\x10\xa2\x93\x04\x12\x1d\n\x17UPLOAD_UNEXPECTED_ERROR\x10\xa3\x93\x04\x12\x14\n\x0eUPLOAD_EXPIRED\x10\xa4\x93\x04\x12\x15\n\x0fUPLOAD_CANCELED\x10\xa5\x93\x04\x12\x15\n\x0fUPLOAD_CONFLICT\x10\xa6\x93\x04\x12\x1a\n\x14\x42ILLING_INVALID_INFO\x10\x88\x9b\x04\x12\x1b\n\x15INTERNAL_SERVER_ISSUE\x10\xd4\xfd\x05\x12\x1d\n\x17INTERNAL_FETCHING_ISSUE\x10\xd5\xfd\x05\x12\x1d\n\x17INTERNAL_DATABASE_ISSUE\x10\xd6\xfd\x05\x12!\n\x1bINTERNAL_UNEXPECTED_TIMEOUT\x10\xd9\xfd\x05\x12\x1c\n\x16INTERNAL_UNEXPECTED_V1\x10\xda\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_PANIC\x10\xdb\xfd\x05\x12\x1f\n\x19INTERNAL_UNEXPECTED_SPIRE\x10\xdc\xfd\x05\x12 \n\x1aINTERNAL_REDIS_UNAVAILABLE\x10\xdd\xfd\x05\x12!\n\x1bINTERNAL_RESOURCE_EXHAUSTED\x10\xde\xfd\x05\x12\"\n\x1cINTERNAL_REDIS_UNCATEGORIZED\x10\xdf\xfd\x05\x12 \n\x1aINTERNAL_AWS_UNCATEGORIZED\x10\xe0\xfd\x05\x12\"\n\x1cINTERNAL_AZURE_UNCATEGORIZED\x10\xe1\xfd\x05\x12\x18\n\x12\x43ONN_UNCATEGORIZED\x10\xb9\x85\x06\x12\x19\n\x13MODEL_UNCATEGORIZED\x10\xba\x85\x06\x12\x19\n\x13INPUT_UNCATEGORIZED\x10\xbb\x85\x06\x12\x1e\n\x18\x41NNOTATION_UNCATEGORIZED\x10\xbc\x85\x06\x12\x1b\n\x15\x42ILLING_UNCATEGORIZED\x10\xbd\x85\x06\x12\x1c\n\x16INTERNAL_UNCATEGORIZED\x10\xc1\x85\x06\x12\x11\n\x0b\x42\x41\x44_REQUEST\x10\xa0\xc2\x05\x12\x12\n\x0cSERVER_ERROR\x10\x84\xc3\x05\"\x08\x08\xbf\xc6\x01\x10\xbf\xc6\x01\"\x08\x08\xe8\x81\x02\x10\xe8\x81\x02\"\x08\x08\xe9\x81\x02\x10\xe9\x81\x02\"\x08\x08\xea\x81\x02\x10\xea\x81\x02\"\x08\x08\xcc\x82\x02\x10\xcc\x82\x02\"\x08\x08\xcd\x82\x02\x10\xcd\x82\x02\"\x08\x08\xce\x82\x02\x10\xce\x82\x02\"\x08\x08\xcf\x82\x02\x10\xcf\x82\x02\"\x08\x08\xd0\x82\x02\x10\xd0\x82\x02\"\x08\x08\xd1\x82\x02\x10\xd1\x82\x02\"\x08\x08\xd2\x82\x02\x10\xd2\x82\x02\"\x08\x08\xb0\x83\x02\x10\xb0\x83\x02\"\x08\x08\xb1\x83\x02\x10\xb1\x83\x02\"\x08\x08\xb3\x83\x02\x10\xb3\x83\x02\"\x08\x08\xba\x83\x02\x10\xba\x83\x02\"\x08\x08\xbb\xb8\x02\x10\xbb\xb8\x02\"\x08\x08\xd2\xb8\x02\x10\xd2\xb8\x02\"\x08\x08\xd3\xb8\x02\x10\xd3\xb8\x02\"\x08\x08\xf0\xc1\x02\x10\xf0\xc1\x02\"\x08\x08\xf1\xc1\x02\x10\xf1\xc1\x02\"\x08\x08\xf2\xc1\x02\x10\xf2\xc1\x02\"\x08\x08\xf3\xc1\x02\x10\xf3\xc1\x02\"\x08\x08\xf4\xc1\x02\x10\xf4\xc1\x02\"\x08\x08\x9c\xc7\x01\x10\x9c\xc7\x01\"\x08\x08\x9d\xc7\x01\x10\x9d\xc7\x01\"\x08\x08\x9e\xc7\x01\x10\x9e\xc7\x01\"\x08\x08\x9f\xc7\x01\x10\x9f\xc7\x01\"\x08\x08\xa1\xc7\x01\x10\xa1\xc7\x01\"\x08\x08\xa2\xc7\x01\x10\xa2\xc7\x01\x42g\n\x1c\x63om.clarifai.grpc.api.statusP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.api.status.status_code_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.clarifai.grpc.api.statusP\001Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/api/status\242\002\004CAIP'
@@ -28,9 +28,9 @@
   _STATUSCODE.values_by_name["MODEL_EVALUATION_MSG_REDELIVER"]._options = None
   _STATUSCODE.values_by_name["MODEL_EVALUATION_MSG_REDELIVER"]._serialized_options = b'\010\001'
   _STATUSCODE.values_by_name["DATA_DUMP_NO_DATA"]._options = None
   _STATUSCODE.values_by_name["DATA_DUMP_NO_DATA"]._serialized_options = b'\010\001'
   _STATUSCODE.values_by_name["INPUT_WRITES_DISABLED_FOR_MAINTENANCE"]._options = None
   _STATUSCODE.values_by_name["INPUT_WRITES_DISABLED_FOR_MAINTENANCE"]._serialized_options = b'\010\001'
   _STATUSCODE._serialized_start=69
-  _STATUSCODE._serialized_end=10769
+  _STATUSCODE._serialized_end=10917
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_code_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_code_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -222,14 +222,20 @@
     """Bulk Operation related codes 254xx"""
     BULK_OPERATION_FAILED: _StatusCode.ValueType  # 25401
     BULK_OPERATION_PENDING: _StatusCode.ValueType  # 25402
     BULK_OPERATION_IN_PROGRESS: _StatusCode.ValueType  # 25403
     BULK_OPERATION_INVALID_REQUEST: _StatusCode.ValueType  # 25404
     BULK_OPERATION_CANCELLED: _StatusCode.ValueType  # 25405
     BULK_OPERATION_UNEXPECTED_ERROR: _StatusCode.ValueType  # 25406
+    RUNNER_DOES_NOT_EXIST: _StatusCode.ValueType  # 25600
+    """Runner related codes 256xx"""
+    RUNNER_PERMISSION_DENIED: _StatusCode.ValueType  # 25601
+    RUNNER_INVALID_ARGUMENT: _StatusCode.ValueType  # 25602
+    RUNNER_INVALID_REQUEST: _StatusCode.ValueType  # 25603
+    RUNNER_NEEDS_RETRY: _StatusCode.ValueType  # 25604
     INPUT_DOWNLOAD_SUCCESS: _StatusCode.ValueType  # 30000
     """Input:Image related 30xxx"""
     INPUT_DOWNLOAD_PENDING: _StatusCode.ValueType  # 30001
     """when things are async, this is the default status."""
     INPUT_DOWNLOAD_FAILED: _StatusCode.ValueType  # 30002
     """any type of error downloading and processing"""
     INPUT_DOWNLOAD_IN_PROGRESS: _StatusCode.ValueType  # 30003
@@ -386,16 +392,18 @@
     """Tasks 54xxx
     The task was created.
     """
     TASK_DONE: _StatusCode.ValueType  # 54002
     """The task is completed."""
     TASK_WONT_DO: _StatusCode.ValueType  # 54003
     """The task is marked as abandoned."""
-    TASK_ADD_ANNOTATIONS_FAILURE: _StatusCode.ValueType  # 54005
-    """An error occurred during add-task-annotations pipeline."""
+    TASK_FAILED: _StatusCode.ValueType  # 54005
+    """An error occurred during add-task-annotations or add-auto-annotations pipeline."""
+    TASK_IDLE: _StatusCode.ValueType  # 54006
+    """When an Auto Annotation task job has finished processing its last batch and is waiting for more dataset assets."""
     TASK_CONFLICT: _StatusCode.ValueType  # 54100
     """The task operation is in conflict with the current state of the server."""
     TASK_NOT_IMPLEMENTED: _StatusCode.ValueType  # 54101
     """Certain task-related scenarios are not implemented."""
     TASK_MISSING: _StatusCode.ValueType  # 54102
     """Task was not found."""
     LABEL_ORDER_PENDING: _StatusCode.ValueType  # 55001
@@ -705,14 +713,20 @@
 """Bulk Operation related codes 254xx"""
 BULK_OPERATION_FAILED: StatusCode.ValueType  # 25401
 BULK_OPERATION_PENDING: StatusCode.ValueType  # 25402
 BULK_OPERATION_IN_PROGRESS: StatusCode.ValueType  # 25403
 BULK_OPERATION_INVALID_REQUEST: StatusCode.ValueType  # 25404
 BULK_OPERATION_CANCELLED: StatusCode.ValueType  # 25405
 BULK_OPERATION_UNEXPECTED_ERROR: StatusCode.ValueType  # 25406
+RUNNER_DOES_NOT_EXIST: StatusCode.ValueType  # 25600
+"""Runner related codes 256xx"""
+RUNNER_PERMISSION_DENIED: StatusCode.ValueType  # 25601
+RUNNER_INVALID_ARGUMENT: StatusCode.ValueType  # 25602
+RUNNER_INVALID_REQUEST: StatusCode.ValueType  # 25603
+RUNNER_NEEDS_RETRY: StatusCode.ValueType  # 25604
 INPUT_DOWNLOAD_SUCCESS: StatusCode.ValueType  # 30000
 """Input:Image related 30xxx"""
 INPUT_DOWNLOAD_PENDING: StatusCode.ValueType  # 30001
 """when things are async, this is the default status."""
 INPUT_DOWNLOAD_FAILED: StatusCode.ValueType  # 30002
 """any type of error downloading and processing"""
 INPUT_DOWNLOAD_IN_PROGRESS: StatusCode.ValueType  # 30003
@@ -869,16 +883,18 @@
 """Tasks 54xxx
 The task was created.
 """
 TASK_DONE: StatusCode.ValueType  # 54002
 """The task is completed."""
 TASK_WONT_DO: StatusCode.ValueType  # 54003
 """The task is marked as abandoned."""
-TASK_ADD_ANNOTATIONS_FAILURE: StatusCode.ValueType  # 54005
-"""An error occurred during add-task-annotations pipeline."""
+TASK_FAILED: StatusCode.ValueType  # 54005
+"""An error occurred during add-task-annotations or add-auto-annotations pipeline."""
+TASK_IDLE: StatusCode.ValueType  # 54006
+"""When an Auto Annotation task job has finished processing its last batch and is waiting for more dataset assets."""
 TASK_CONFLICT: StatusCode.ValueType  # 54100
 """The task operation is in conflict with the current state of the server."""
 TASK_NOT_IMPLEMENTED: StatusCode.ValueType  # 54101
 """Certain task-related scenarios are not implemented."""
 TASK_MISSING: StatusCode.ValueType  # 54102
 """Task was not found."""
 LABEL_ORDER_PENDING: StatusCode.ValueType  # 55001
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/status/status_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/status/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/extensions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/matrix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/test_proto_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/api/utils/test_proto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/scope/scope_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%proto/clarifai/auth/scope/scope.proto\x12\x13\x63larifai.auth.scope\x1a google/protobuf/descriptor.proto\"F\n\tScopeList\x12&\n\x06scopes\x18\x01 \x03(\x0e\x32\x16.clarifai.auth.scope.S\x12\x11\n\tendpoints\x18\x02 \x03(\t*\xe6\x14\n\x01S\x12\t\n\x05undef\x10\x00\x12\r\n\x03\x41ll\x10\x01\x1a\x04\xf0\x9b\'\x01\x12\x11\n\x07Predict\x10\x02\x1a\x04\xf0\x9b\'\x01\x12\x18\n\nInputs_Add\x10\x04\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x05\x12\x14\n\nInputs_Get\x10\x05\x1a\x04\xf0\x9b\'\x01\x12 \n\x0cInputs_Patch\x10\x07\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\x04\xf8\x9b\'\x05\x12\x1f\n\rInputs_Delete\x10\x08\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'\x04\xf8\x9b\'\x05\x12\x1d\n\rOutputs_Patch\x10\t\x1a\n\x08\x01\xf8\x9b\'\x05\xf8\x9b\'\x02\x12\x1a\n\x0c\x43oncepts_Add\x10\n\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x0b\x12\x16\n\x0c\x43oncepts_Get\x10\x0b\x1a\x04\xf0\x9b\'\x01\x12\"\n\x0e\x43oncepts_Patch\x10\x0c\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\n\xf8\x9b\'\x0b\x12\x1d\n\x0f\x43oncepts_Delete\x10\r\x1a\x08\xf8\x9b\'\n\xf8\x9b\'\x0b\x12\x18\n\nModels_Add\x10\x0e\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x0f\x12\x14\n\nModels_Get\x10\x0f\x1a\x04\xf0\x9b\'\x01\x12$\n\x0cModels_Patch\x10\x10\x1a\x12\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\x0e\xf8\x9b\'\x0f\xf8\x9b\'\x1a\x12\x1f\n\rModels_Delete\x10\x11\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'\x0e\xf8\x9b\'\x0f\x12\x1a\n\x0cModels_Train\x10\x1a\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x0f\x12\x15\n\x0bModels_Sync\x10\x1b\x1a\x04\xf8\x9b\'\x0f\x12\x1b\n\rWorkflows_Add\x10\x12\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x13\x12\x17\n\rWorkflows_Get\x10\x13\x1a\x04\xf0\x9b\'\x01\x12#\n\x0fWorkflows_Patch\x10\x14\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\x12\xf8\x9b\'\x13\x12\"\n\x10Workflows_Delete\x10\x15\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'\x12\xf8\x9b\'\x13\x12\x1d\n\x13WorkflowMetrics_Get\x10`\x1a\x04\xf0\x9b\'\x01\x12!\n\x13WorkflowMetrics_Add\x10\x61\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'`\x12(\n\x16WorkflowMetrics_Delete\x10\x62\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'a\xf8\x9b\'`\x12\"\n\x16TSNEVisualizations_Add\x10\x18\x1a\x06\x08\x01\xf8\x9b\'\x19\x12\x1e\n\x16TSNEVisualizations_Get\x10\x19\x1a\x02\x08\x01\x12\x1d\n\x0f\x41nnotations_Add\x10%\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'&\x12\x19\n\x0f\x41nnotations_Get\x10&\x1a\x04\xf0\x9b\'\x01\x12%\n\x11\x41nnotations_Patch\x10\'\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'%\xf8\x9b\'&\x12$\n\x12\x41nnotations_Delete\x10(\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'%\xf8\x9b\'&\x12\x1c\n\x0e\x43ollectors_Add\x10)\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'*\x12\x18\n\x0e\x43ollectors_Get\x10*\x1a\x04\xf0\x9b\'\x01\x12#\n\x11\x43ollectors_Delete\x10+\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\')\xf8\x9b\'*\x12\x16\n\x08\x41pps_Add\x10,\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'-\x12\x12\n\x08\x41pps_Get\x10-\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0b\x41pps_Delete\x10.\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\',\xf8\x9b\'-\x12\x16\n\x08Keys_Add\x10/\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'0\x12\x12\n\x08Keys_Get\x10\x30\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0bKeys_Delete\x10\x31\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'/\xf8\x9b\'0\x12\x1f\n\x11\x43ollaborators_Add\x10\x33\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'2\x12\x1b\n\x11\x43ollaborators_Get\x10\x32\x1a\x04\xf0\x9b\'\x01\x12&\n\x14\x43ollaborators_Delete\x10\x34\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'3\xf8\x9b\'2\x12\x19\n\x0bMetrics_Add\x10\x36\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'5\x12\x15\n\x0bMetrics_Get\x10\x35\x1a\x04\xf0\x9b\'\x01\x12 \n\x0eMetrics_Delete\x10?\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'6\xf8\x9b\'5\x12\x17\n\tTasks_Add\x10\x37\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'8\x12\x13\n\tTasks_Get\x10\x38\x1a\x04\xf0\x9b\'\x01\x12\x1e\n\x0cTasks_Delete\x10\x46\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'7\xf8\x9b\'8\x12\"\n\x14PasswordPolicies_Add\x10\x39\x1a\x08\xf0\x9b\'\x01\xf8\x9b\':\x12\x1e\n\x14PasswordPolicies_Get\x10:\x1a\x04\xf0\x9b\'\x01\x12)\n\x17PasswordPolicies_Delete\x10;\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'9\xf8\x9b\':\x12\x19\n\x0fLabelOrders_Get\x10\x43\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0fLabelOrders_Add\x10\x44\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'C\x12$\n\x12LabelOrders_Delete\x10\x45\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'D\xf8\x9b\'C\x12 \n\x16UserFeatureConfigs_Get\x10G\x1a\x04\xf0\x9b\'\x01\x12.\n FindDuplicateAnnotationsJobs_Add\x10\x66\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'g\x12*\n FindDuplicateAnnotationsJobs_Get\x10g\x1a\x04\xf0\x9b\'\x01\x12\x35\n#FindDuplicateAnnotationsJobs_Delete\x10h\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'f\xf8\x9b\'g\x12\x16\n\x0c\x44\x61tasets_Get\x10i\x1a\x04\xf0\x9b\'\x01\x12\x1a\n\x0c\x44\x61tasets_Add\x10j\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'i\x12!\n\x0f\x44\x61tasets_Delete\x10k\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'i\xf8\x9b\'j\x12\x19\n\x0bModules_Add\x10l\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'m\x12\x15\n\x0bModules_Get\x10m\x1a\x04\xf0\x9b\'\x01\x12 \n\x0eModules_Delete\x10n\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'l\xf8\x9b\'m\x12-\n\x1bInstalledModuleVersions_Add\x10o\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'p\xf8\x9b\'m\x12)\n\x1bInstalledModuleVersions_Get\x10p\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'m\x12\x34\n\x1eInstalledModuleVersions_Delete\x10q\x1a\x10\xf0\x9b\'\x01\xf8\x9b\'o\xf8\x9b\'p\xf8\x9b\'m\x12\x10\n\x06Search\x10\x03\x1a\x04\xf0\x9b\'\x01\x12\x19\n\x0fSavedSearch_Get\x10r\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0fSavedSearch_Add\x10s\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'r\x12$\n\x12SavedSearch_Delete\x10t\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'r\xf8\x9b\'s\x12&\n\x1cModelVersionPublications_Add\x10u\x1a\x04\xf0\x9b\'\x01\x12)\n\x1fModelVersionPublications_Delete\x10v\x1a\x04\xf0\x9b\'\x01\x12\"\n\x18WorkflowPublications_Add\x10w\x1a\x04\xf0\x9b\'\x01\x12%\n\x1bWorkflowPublications_Delete\x10x\x1a\x04\xf0\x9b\'\x01\x12\x1f\n\x11\x42ulkOperation_Add\x10y\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'z\x12\x1b\n\x11\x42ulkOperation_Get\x10z\x1a\x04\xf0\x9b\'\x01\x12&\n\x14\x42ulkOperation_Delete\x10{\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'y\xf8\x9b\'z\x12\x17\n\x13HistoricalUsage_Get\x10|\x12\x16\n\x0bUploads_Get\x10\x80\x01\x1a\x04\xf0\x9b\'\x01\x12\x1b\n\x0bUploads_Add\x10\x81\x01\x1a\t\xf0\x9b\'\x01\xf8\x9b\'\x80\x01\x12#\n\x0eUploads_Delete\x10\x82\x01\x1a\x0e\xf0\x9b\'\x01\xf8\x9b\'\x80\x01\xf8\x9b\'\x81\x01\"\x04\x08\x1e\x10\x1e\"\x04\x08\x1f\x10\x1f\"\x04\x08 \x10 \"\x04\x08!\x10!\"\x04\x08\"\x10\"\"\x04\x08}\x10}\"\x04\x08~\x10~:<\n\x0f\x63larfai_exposed\x12!.google.protobuf.EnumValueOptions\x18\xbe\xf3\x04 \x01(\x08:^\n\x19\x63larifai_depending_scopes\x12!.google.protobuf.EnumValueOptions\x18\xbf\xf3\x04 \x03(\x0e\x32\x16.clarifai.auth.scope.SBg\n\x1c\x63om.clarifai.grpc.auth.scopeP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/auth/scope\xa2\x02\x04\x43\x41IPb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%proto/clarifai/auth/scope/scope.proto\x12\x13\x63larifai.auth.scope\x1a google/protobuf/descriptor.proto\"F\n\tScopeList\x12&\n\x06scopes\x18\x01 \x03(\x0e\x32\x16.clarifai.auth.scope.S\x12\x11\n\tendpoints\x18\x02 \x03(\t*\xfd\x15\n\x01S\x12\t\n\x05undef\x10\x00\x12\r\n\x03\x41ll\x10\x01\x1a\x04\xf0\x9b\'\x01\x12\x11\n\x07Predict\x10\x02\x1a\x04\xf0\x9b\'\x01\x12\x18\n\nInputs_Add\x10\x04\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x05\x12\x14\n\nInputs_Get\x10\x05\x1a\x04\xf0\x9b\'\x01\x12 \n\x0cInputs_Patch\x10\x07\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\x04\xf8\x9b\'\x05\x12\x1f\n\rInputs_Delete\x10\x08\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'\x04\xf8\x9b\'\x05\x12\x1d\n\rOutputs_Patch\x10\t\x1a\n\x08\x01\xf8\x9b\'\x05\xf8\x9b\'\x02\x12\x1a\n\x0c\x43oncepts_Add\x10\n\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x0b\x12\x16\n\x0c\x43oncepts_Get\x10\x0b\x1a\x04\xf0\x9b\'\x01\x12\"\n\x0e\x43oncepts_Patch\x10\x0c\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\n\xf8\x9b\'\x0b\x12\x1d\n\x0f\x43oncepts_Delete\x10\r\x1a\x08\xf8\x9b\'\n\xf8\x9b\'\x0b\x12\x18\n\nModels_Add\x10\x0e\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x0f\x12\x14\n\nModels_Get\x10\x0f\x1a\x04\xf0\x9b\'\x01\x12$\n\x0cModels_Patch\x10\x10\x1a\x12\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\x0e\xf8\x9b\'\x0f\xf8\x9b\'\x1a\x12\x1f\n\rModels_Delete\x10\x11\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'\x0e\xf8\x9b\'\x0f\x12\x1a\n\x0cModels_Train\x10\x1a\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x0f\x12\x15\n\x0bModels_Sync\x10\x1b\x1a\x04\xf8\x9b\'\x0f\x12\x1b\n\rWorkflows_Add\x10\x12\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'\x13\x12\x17\n\rWorkflows_Get\x10\x13\x1a\x04\xf0\x9b\'\x01\x12#\n\x0fWorkflows_Patch\x10\x14\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'\x12\xf8\x9b\'\x13\x12\"\n\x10Workflows_Delete\x10\x15\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'\x12\xf8\x9b\'\x13\x12\x1d\n\x13WorkflowMetrics_Get\x10`\x1a\x04\xf0\x9b\'\x01\x12!\n\x13WorkflowMetrics_Add\x10\x61\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'`\x12(\n\x16WorkflowMetrics_Delete\x10\x62\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'a\xf8\x9b\'`\x12\"\n\x16TSNEVisualizations_Add\x10\x18\x1a\x06\x08\x01\xf8\x9b\'\x19\x12\x1e\n\x16TSNEVisualizations_Get\x10\x19\x1a\x02\x08\x01\x12\x1d\n\x0f\x41nnotations_Add\x10%\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'&\x12\x19\n\x0f\x41nnotations_Get\x10&\x1a\x04\xf0\x9b\'\x01\x12%\n\x11\x41nnotations_Patch\x10\'\x1a\x0e\x08\x01\xf0\x9b\'\x01\xf8\x9b\'%\xf8\x9b\'&\x12$\n\x12\x41nnotations_Delete\x10(\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'%\xf8\x9b\'&\x12\x1c\n\x0e\x43ollectors_Add\x10)\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'*\x12\x18\n\x0e\x43ollectors_Get\x10*\x1a\x04\xf0\x9b\'\x01\x12#\n\x11\x43ollectors_Delete\x10+\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\')\xf8\x9b\'*\x12\x16\n\x08\x41pps_Add\x10,\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'-\x12\x12\n\x08\x41pps_Get\x10-\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0b\x41pps_Delete\x10.\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\',\xf8\x9b\'-\x12\x16\n\x08Keys_Add\x10/\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'0\x12\x12\n\x08Keys_Get\x10\x30\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0bKeys_Delete\x10\x31\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'/\xf8\x9b\'0\x12\x1f\n\x11\x43ollaborators_Add\x10\x33\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'2\x12\x1b\n\x11\x43ollaborators_Get\x10\x32\x1a\x04\xf0\x9b\'\x01\x12&\n\x14\x43ollaborators_Delete\x10\x34\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'3\xf8\x9b\'2\x12\x19\n\x0bMetrics_Add\x10\x36\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'5\x12\x15\n\x0bMetrics_Get\x10\x35\x1a\x04\xf0\x9b\'\x01\x12 \n\x0eMetrics_Delete\x10?\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'6\xf8\x9b\'5\x12\x17\n\tTasks_Add\x10\x37\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'8\x12\x13\n\tTasks_Get\x10\x38\x1a\x04\xf0\x9b\'\x01\x12\x1e\n\x0cTasks_Delete\x10\x46\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'7\xf8\x9b\'8\x12\"\n\x14PasswordPolicies_Add\x10\x39\x1a\x08\xf0\x9b\'\x01\xf8\x9b\':\x12\x1e\n\x14PasswordPolicies_Get\x10:\x1a\x04\xf0\x9b\'\x01\x12)\n\x17PasswordPolicies_Delete\x10;\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'9\xf8\x9b\':\x12\x19\n\x0fLabelOrders_Get\x10\x43\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0fLabelOrders_Add\x10\x44\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'C\x12$\n\x12LabelOrders_Delete\x10\x45\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'D\xf8\x9b\'C\x12 \n\x16UserFeatureConfigs_Get\x10G\x1a\x04\xf0\x9b\'\x01\x12.\n FindDuplicateAnnotationsJobs_Add\x10\x66\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'g\x12*\n FindDuplicateAnnotationsJobs_Get\x10g\x1a\x04\xf0\x9b\'\x01\x12\x35\n#FindDuplicateAnnotationsJobs_Delete\x10h\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'f\xf8\x9b\'g\x12\x16\n\x0c\x44\x61tasets_Get\x10i\x1a\x04\xf0\x9b\'\x01\x12\x1a\n\x0c\x44\x61tasets_Add\x10j\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'i\x12!\n\x0f\x44\x61tasets_Delete\x10k\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'i\xf8\x9b\'j\x12\x19\n\x0bModules_Add\x10l\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'m\x12\x15\n\x0bModules_Get\x10m\x1a\x04\xf0\x9b\'\x01\x12 \n\x0eModules_Delete\x10n\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'l\xf8\x9b\'m\x12-\n\x1bInstalledModuleVersions_Add\x10o\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'p\xf8\x9b\'m\x12)\n\x1bInstalledModuleVersions_Get\x10p\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'m\x12\x34\n\x1eInstalledModuleVersions_Delete\x10q\x1a\x10\xf0\x9b\'\x01\xf8\x9b\'o\xf8\x9b\'p\xf8\x9b\'m\x12\x10\n\x06Search\x10\x03\x1a\x04\xf0\x9b\'\x01\x12\x19\n\x0fSavedSearch_Get\x10r\x1a\x04\xf0\x9b\'\x01\x12\x1d\n\x0fSavedSearch_Add\x10s\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'r\x12$\n\x12SavedSearch_Delete\x10t\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'r\xf8\x9b\'s\x12&\n\x1cModelVersionPublications_Add\x10u\x1a\x04\xf0\x9b\'\x01\x12)\n\x1fModelVersionPublications_Delete\x10v\x1a\x04\xf0\x9b\'\x01\x12\"\n\x18WorkflowPublications_Add\x10w\x1a\x04\xf0\x9b\'\x01\x12%\n\x1bWorkflowPublications_Delete\x10x\x1a\x04\xf0\x9b\'\x01\x12\x1f\n\x11\x42ulkOperation_Add\x10y\x1a\x08\xf0\x9b\'\x01\xf8\x9b\'z\x12\x1b\n\x11\x42ulkOperation_Get\x10z\x1a\x04\xf0\x9b\'\x01\x12&\n\x14\x42ulkOperation_Delete\x10{\x1a\x0c\xf0\x9b\'\x01\xf8\x9b\'y\xf8\x9b\'z\x12\x17\n\x13HistoricalUsage_Get\x10|\x12\x16\n\x0bUploads_Get\x10\x80\x01\x1a\x04\xf0\x9b\'\x01\x12\x1b\n\x0bUploads_Add\x10\x81\x01\x1a\t\xf0\x9b\'\x01\xf8\x9b\'\x80\x01\x12#\n\x0eUploads_Delete\x10\x82\x01\x1a\x0e\xf0\x9b\'\x01\xf8\x9b\'\x80\x01\xf8\x9b\'\x81\x01\x12\x16\n\x0bRunners_Get\x10\x83\x01\x1a\x04\xf0\x9b\'\x01\x12\x1b\n\x0bRunners_Add\x10\x84\x01\x1a\t\xf0\x9b\'\x01\xf8\x9b\'\x83\x01\x12#\n\x0eRunners_Delete\x10\x85\x01\x1a\x0e\xf0\x9b\'\x01\xf8\x9b\'\x83\x01\xf8\x9b\'\x84\x01\x12\x1a\n\x0fRunnerItems_Get\x10\x86\x01\x1a\x04\xf0\x9b\'\x01\x12\x1f\n\x0fRunnerItems_Add\x10\x87\x01\x1a\t\xf0\x9b\'\x01\xf8\x9b\'\x86\x01\"\x04\x08\x1e\x10\x1e\"\x04\x08\x1f\x10\x1f\"\x04\x08 \x10 \"\x04\x08!\x10!\"\x04\x08\"\x10\"\"\x04\x08}\x10}\"\x04\x08~\x10~:<\n\x0f\x63larfai_exposed\x12!.google.protobuf.EnumValueOptions\x18\xbe\xf3\x04 \x01(\x08:^\n\x19\x63larifai_depending_scopes\x12!.google.protobuf.EnumValueOptions\x18\xbf\xf3\x04 \x03(\x0e\x32\x16.clarifai.auth.scope.SBg\n\x1c\x63om.clarifai.grpc.auth.scopeP\x01Z>github.com/Clarifai/clarifai-go-grpc/proto/clarifai/auth/scope\xa2\x02\x04\x43\x41IPb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.clarifai.auth.scope.scope_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.EnumValueOptions.RegisterExtension(clarfai_exposed)
   google_dot_protobuf_dot_descriptor__pb2.EnumValueOptions.RegisterExtension(clarifai_depending_scopes)
 
@@ -182,12 +182,22 @@
   _S.values_by_name["BulkOperation_Delete"]._serialized_options = b'\360\233\'\001\370\233\'y\370\233\'z'
   _S.values_by_name["Uploads_Get"]._options = None
   _S.values_by_name["Uploads_Get"]._serialized_options = b'\360\233\'\001'
   _S.values_by_name["Uploads_Add"]._options = None
   _S.values_by_name["Uploads_Add"]._serialized_options = b'\360\233\'\001\370\233\'\200\001'
   _S.values_by_name["Uploads_Delete"]._options = None
   _S.values_by_name["Uploads_Delete"]._serialized_options = b'\360\233\'\001\370\233\'\200\001\370\233\'\201\001'
+  _S.values_by_name["Runners_Get"]._options = None
+  _S.values_by_name["Runners_Get"]._serialized_options = b'\360\233\'\001'
+  _S.values_by_name["Runners_Add"]._options = None
+  _S.values_by_name["Runners_Add"]._serialized_options = b'\360\233\'\001\370\233\'\203\001'
+  _S.values_by_name["Runners_Delete"]._options = None
+  _S.values_by_name["Runners_Delete"]._serialized_options = b'\360\233\'\001\370\233\'\203\001\370\233\'\204\001'
+  _S.values_by_name["RunnerItems_Get"]._options = None
+  _S.values_by_name["RunnerItems_Get"]._serialized_options = b'\360\233\'\001'
+  _S.values_by_name["RunnerItems_Add"]._options = None
+  _S.values_by_name["RunnerItems_Add"]._serialized_options = b'\360\233\'\001\370\233\'\206\001'
   _S._serialized_start=169
-  _S._serialized_end=2831
+  _S._serialized_end=2982
   _SCOPELIST._serialized_start=96
   _SCOPELIST._serialized_end=166
 # @@protoc_insertion_point(module_scope)
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/scope/scope_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -202,14 +202,20 @@
     HistoricalUsage_Get: _S.ValueType  # 124
     """To read historical usage from usage.dashboard_items table"""
     Uploads_Get: _S.ValueType  # 128
     """To read uploaded files and archives info from Uploads endpoints"""
     Uploads_Add: _S.ValueType  # 129
     """To upload files or archives through the Uploads endpoints"""
     Uploads_Delete: _S.ValueType  # 130
+    Runners_Get: _S.ValueType  # 131
+    """To read allo control over remote runners"""
+    Runners_Add: _S.ValueType  # 132
+    Runners_Delete: _S.ValueType  # 133
+    RunnerItems_Get: _S.ValueType  # 134
+    RunnerItems_Add: _S.ValueType  # 135
 
 class S(_S, metaclass=_SEnumTypeWrapper):
     """Next index: 41
     NOTE: When updating the list of "clarifai_exposed" scopes, please also
     update the TestScopes function in main_key_test.go and TestGetExposedScopes function in
     scope_test.go
 
@@ -413,14 +419,20 @@
 HistoricalUsage_Get: S.ValueType  # 124
 """To read historical usage from usage.dashboard_items table"""
 Uploads_Get: S.ValueType  # 128
 """To read uploaded files and archives info from Uploads endpoints"""
 Uploads_Add: S.ValueType  # 129
 """To upload files or archives through the Uploads endpoints"""
 Uploads_Delete: S.ValueType  # 130
+Runners_Get: S.ValueType  # 131
+"""To read allo control over remote runners"""
+Runners_Add: S.ValueType  # 132
+Runners_Delete: S.ValueType  # 133
+RunnerItems_Get: S.ValueType  # 134
+RunnerItems_Add: S.ValueType  # 135
 global___S = S
 
 @typing_extensions.final
 class ScopeList(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SCOPES_FIELD_NUMBER: builtins.int
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/types/types_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.py` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/util/extension_pb2.py`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc/grpc/auth/util/extension_pb2.pyi` & `clarifai-grpc-9.6.1/clarifai_grpc/grpc/auth/util/extension_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc.egg-info/PKG-INFO` & `clarifai-grpc-9.6.1/clarifai_grpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai-grpc
-Version: 9.6.0
+Version: 9.6.1
 Summary: Clarifai gRPC API Client
 Home-page: https://github.com/Clarifai/clarifai-python-grpc
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-grpc-9.6.0/clarifai_grpc.egg-info/SOURCES.txt` & `clarifai-grpc-9.6.1/clarifai_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clarifai-grpc-9.6.0/setup.py` & `clarifai-grpc-9.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_packages(include=["clarifai_grpc*"])
 
 setuptools.setup(
     name="clarifai-grpc",
-    version="9.6.0",
+    version="9.6.1",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai gRPC API Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-grpc",
     packages=packages,
```

