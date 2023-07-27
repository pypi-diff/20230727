# Comparing `tmp/messageflux-0.3.0.tar.gz` & `tmp/messageflux-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messageflux-0.3.0.tar", last modified: Mon Jul 24 14:58:35 2023, max compression
+gzip compressed data, was "messageflux-0.3.1.tar", last modified: Thu Jul 27 17:34:32 2023, max compression
```

## Comparing `messageflux-0.3.0.tar` & `messageflux-0.3.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.285151 messageflux-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-24 14:58:21.000000 messageflux-0.3.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 14:58:21.000000 messageflux-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 14:58:21.000000 messageflux-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-24 14:58:35.285151 messageflux-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-24 14:58:21.000000 messageflux-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 14:58:22.000000 messageflux-0.3.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.273151 messageflux-0.3.0/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:21.000000 messageflux-0.3.0/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 14:58:21.000000 messageflux-0.3.0/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 14:58:21.000000 messageflux-0.3.0/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/fastmessage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/base/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/input_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/input_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/base/output_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/file_system/file_system_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux/iodevices/in_memory_device/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/in_memory_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3_message_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/fs_poison_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/LogType.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/bulk_rotating_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/bulk_rotating_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/bulk_rotating_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/logging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/message_handling_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/metadata_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/multiprocessing/multiprocessrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/multiprocessing/singleprocesshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/pipeline_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/server_loop_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.281151 messageflux-0.3.0/messageflux/service_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/service_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/service_addons/loop_health_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.285151 messageflux-0.3.0/messageflux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-24 14:58:21.000000 messageflux-0.3.0/messageflux/utils/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 14:58:35.277151 messageflux-0.3.0/messageflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 14:58:35.000000 messageflux-0.3.0/messageflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 14:58:21.000000 messageflux-0.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-24 14:58:21.000000 messageflux-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 14:58:21.000000 messageflux-0.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 14:58:35.000000 messageflux-0.3.0/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-fastmessage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-objectstorage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements-rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 14:58:21.000000 messageflux-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 14:58:35.285151 messageflux-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 17:34:19.000000 messageflux-0.3.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 17:34:19.000000 messageflux-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-27 17:34:19.000000 messageflux-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-27 17:34:32.725883 messageflux-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-27 17:34:19.000000 messageflux-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 17:34:21.000000 messageflux-0.3.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.713882 messageflux-0.3.1/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:19.000000 messageflux-0.3.1/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 17:34:19.000000 messageflux-0.3.1/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-27 17:34:19.000000 messageflux-0.3.1/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/fastmessage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/input_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/input_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/base/output_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/file_system/file_system_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux/iodevices/in_memory_device/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/in_memory_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3_message_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/fs_poison_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.721882 messageflux-0.3.1/messageflux/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/LogType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/bulk_rotating_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/bulk_rotating_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/bulk_rotating_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/logging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/message_handling_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/metadata_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/messageflux/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/multiprocessing/multiprocessrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/multiprocessing/singleprocesshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/pipeline_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/server_loop_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/messageflux/service_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/service_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/service_addons/loop_health_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.725883 messageflux-0.3.1/messageflux/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-27 17:34:19.000000 messageflux-0.3.1/messageflux/utils/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:34:32.717882 messageflux-0.3.1/messageflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 17:34:32.000000 messageflux-0.3.1/messageflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 17:34:19.000000 messageflux-0.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-27 17:34:19.000000 messageflux-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 17:34:19.000000 messageflux-0.3.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 17:34:32.000000 messageflux-0.3.1/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-fastmessage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-objectstorage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements-rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:34:19.000000 messageflux-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:34:32.725883 messageflux-0.3.1/setup.cfg
```

### Comparing `messageflux-0.3.0/LICENSE` & `messageflux-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/PKG-INFO` & `messageflux-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.0
+Version: 0.3.1
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.3.0/README.md` & `messageflux-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/_custom_build/make_all_extra_requirements.py` & `messageflux-0.3.1/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/base_service.py` & `messageflux-0.3.1/messageflux/base_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/fastmessage_handler.py` & `messageflux-0.3.1/messageflux/fastmessage_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,23 @@
 class MultipleReturnValues(list):
     """
     a value that indicates that multiple output values should be returned
     """
     pass
 
 
+@dataclass
+class FastMessageOutput:
+    """
+    a result that contains the output device name to send the value to
+    """
+    output_device: str
+    value: Any
+
+
 class _DefaultClass(str):
     pass
 
 
 _DEFAULT = _DefaultClass()
 _CALLABLE_TYPE = TypeVar('_CALLABLE_TYPE', bound=Callable[..., Any])
 
@@ -132,29 +141,40 @@
             model = parse_raw_as(self._model, message_bundle.message.bytes)
             kwargs.update(dict(model))
 
         callback_return = self._callback(**kwargs)
         if callback_return is None:
             return None
 
-        if self._output_device is None:
-            _logger.warning(f"callback for input device '{input_device.name}' returned value, "
-                            f"but is not mapped to output device")
-            return None
+        return self._get_pipeline_results(value=callback_return,
+                                          default_output_device=self._output_device)
+
+    def _get_pipeline_results(self, value: Any, default_output_device: Optional[str]) -> List[PipelineResult]:
         results = []
-        if isinstance(callback_return, MultipleReturnValues):
-            return_list: List[Any] = callback_return
+        if isinstance(value, MultipleReturnValues):
+            for item in value:
+                results.extend(self._get_pipeline_results(value=item,
+                                                          default_output_device=default_output_device))
+        elif isinstance(value, FastMessageOutput):
+            results.extend(self._get_pipeline_results(value=value.value,
+                                                      default_output_device=value.output_device))
         else:
-            return_list = [callback_return]
-        for return_value in return_list:
-            results.append(self._get_single_pipeline_result(return_value, self._output_device))
+            pipeline_result = self._get_single_pipeline_result(value=value,
+                                                               output_device=default_output_device)
+            if pipeline_result is not None:
+                results.append(pipeline_result)
 
         return results
 
-    def _get_single_pipeline_result(self, value: Any, output_device: str):
+    def _get_single_pipeline_result(self, value: Any, output_device: Optional[str]) -> Optional[PipelineResult]:
+        if output_device is None:
+            _logger.warning(f"callback for input device '{self._input_device}' returned value, "
+                            f"but is not mapped to output device")
+            return None
+
         if isinstance(value, MessageBundle):
             output_bundle = value
         elif isinstance(value, Message):
             output_bundle = MessageBundle(message=value)
         else:
             json_encoder = getattr(value, '__json_encoder__', BaseModel.__json_encoder__)
             output_data = json.dumps(value, default=json_encoder).encode()
@@ -163,15 +183,15 @@
         return PipelineResult(output_device_name=output_device, message_bundle=output_bundle)
 
 
 class FastMessage(PipelineHandlerBase):
     def __init__(self, default_output_device: Optional[str] = None,
                  validation_error_handler: Optional[Callable[
                      [InputDevice, MessageBundle, ValidationError],
-                     Optional[PipelineResult]]] = None):
+                     Optional[Union[PipelineResult, List[PipelineResult]]]]] = None):
         """
 
         :param default_output_device: an optional default output device to send callaback results to,
         unless mapped otherwise
         :param validation_error_handler: an optional handler that will be called on validation errors,
         in order to give the user a chance to handle them gracefully
         """
```

### Comparing `messageflux-0.3.0/messageflux/iodevices/base/__init__.py` & `messageflux-0.3.1/messageflux/iodevices/base/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/base/common.py` & `messageflux-0.3.1/messageflux/iodevices/base/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/base/input_devices.py` & `messageflux-0.3.1/messageflux/iodevices/base/input_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/base/input_transaction.py` & `messageflux-0.3.1/messageflux/iodevices/base/input_transaction.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/base/output_devices.py` & `messageflux-0.3.1/messageflux/iodevices/base/output_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_input_device.py` & `messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/collection_device_wrapper/collection_output_device.py` & `messageflux-0.3.1/messageflux/iodevices/collection_device_wrapper/collection_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py` & `messageflux-0.3.1/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/file_system/__init__.py` & `messageflux-0.3.1/messageflux/iodevices/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_device_manager_base.py` & `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_input_device.py` & `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_output_device.py` & `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/file_system/file_system_serializer.py` & `messageflux-0.3.1/messageflux/iodevices/file_system/file_system_serializer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/in_memory_device/in_memory_device_manager.py` & `messageflux-0.3.1/messageflux/iodevices/in_memory_device/in_memory_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py` & `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_base.py` & `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py` & `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py` & `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py` & `messageflux-0.3.1/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/objectstorage/s3_message_store.py` & `messageflux-0.3.1/messageflux/iodevices/objectstorage/s3_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3bucket.py` & `messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3bucket.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/objectstorage/s3api/s3client.py` & `messageflux-0.3.1/messageflux/iodevices/objectstorage/s3api/s3client.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/rabbitmq/fs_poison_counter.py` & `messageflux-0.3.1/messageflux/iodevices/rabbitmq/fs_poison_counter.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py` & `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py` & `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py` & `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py` & `messageflux-0.3.1/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py` & `messageflux-0.3.1/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/common.py` & `messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py` & `messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py` & `messageflux-0.3.1/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py` & `messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py` & `messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py` & `messageflux-0.3.1/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/logging/bulk_rotating_device_handler.py` & `messageflux-0.3.1/messageflux/logging/bulk_rotating_device_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/logging/bulk_rotating_file_handler.py` & `messageflux-0.3.1/messageflux/logging/bulk_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/logging/bulk_rotating_handler_base.py` & `messageflux-0.3.1/messageflux/logging/bulk_rotating_handler_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/message_handling_service.py` & `messageflux-0.3.1/messageflux/message_handling_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/multiprocessing/multiprocessrunner.py` & `messageflux-0.3.1/messageflux/multiprocessing/multiprocessrunner.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/multiprocessing/singleprocesshandler.py` & `messageflux-0.3.1/messageflux/multiprocessing/singleprocesshandler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/pipeline_service.py` & `messageflux-0.3.1/messageflux/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/server_loop_service.py` & `messageflux-0.3.1/messageflux/server_loop_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/service_addons/loop_health_addon.py` & `messageflux-0.3.1/messageflux/service_addons/loop_health_addon.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/utils/__init__.py` & `messageflux-0.3.1/messageflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/utils/context.py` & `messageflux-0.3.1/messageflux/utils/context.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux/utils/filesystem.py` & `messageflux-0.3.1/messageflux/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/messageflux.egg-info/PKG-INFO` & `messageflux-0.3.1/messageflux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.0
+Version: 0.3.1
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `messageflux-0.3.0/messageflux.egg-info/SOURCES.txt` & `messageflux-0.3.1/messageflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.0/pyproject.toml` & `messageflux-0.3.1/pyproject.toml`

 * *Files identical despite different names*

