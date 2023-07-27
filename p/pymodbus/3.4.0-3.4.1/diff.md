# Comparing `tmp/pymodbus-3.4.0.tar.gz` & `tmp/pymodbus-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodbus-3.4.0.tar", last modified: Thu Jul 20 12:31:08 2023, max compression
+gzip compressed data, was "pymodbus-3.4.1.tar", last modified: Thu Jul 27 15:27:06 2023, max compression
```

## Comparing `pymodbus-3.4.0.tar` & `pymodbus-3.4.1.tar`

### file list

```diff
@@ -1,135 +1,134 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.408580 pymodbus-3.4.0/
--rw-r--r--   0 jan        (501) staff       (20)    28645 2023-07-20 12:09:25.000000 pymodbus-3.4.0/CHANGELOG.rst
--rw-r--r--   0 jan        (501) staff       (20)     1392 2023-07-20 10:02:40.000000 pymodbus-3.4.0/LICENSE
--rw-r--r--   0 jan        (501) staff       (20)       82 2023-07-20 10:02:40.000000 pymodbus-3.4.0/MANIFEST.in
--rw-r--r--   0 jan        (501) staff       (20)    12723 2023-07-20 12:31:08.408671 pymodbus-3.4.0/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)    11229 2023-07-20 12:09:40.000000 pymodbus-3.4.0/README.rst
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.397452 pymodbus-3.4.0/pymodbus/
--rw-r--r--   0 jan        (501) staff       (20)      316 2023-07-20 12:10:15.000000 pymodbus-3.4.0/pymodbus/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     9422 2023-07-20 12:10:28.000000 pymodbus-3.4.0/pymodbus/bit_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)     9532 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/bit_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.399142 pymodbus-3.4.0/pymodbus/client/
--rw-r--r--   0 jan        (501) staff       (20)      602 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    12304 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/base.py
--rw-r--r--   0 jan        (501) staff       (20)    21046 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/client/mixin.py
--rw-r--r--   0 jan        (501) staff       (20)     9723 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/serial.py
--rw-r--r--   0 jan        (501) staff       (20)     9337 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/tcp.py
--rw-r--r--   0 jan        (501) staff       (20)     5779 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/tls.py
--rw-r--r--   0 jan        (501) staff       (20)     5629 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/client/udp.py
--rw-r--r--   0 jan        (501) staff       (20)     3982 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/constants.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.399712 pymodbus-3.4.0/pymodbus/datastore/
--rw-r--r--   0 jan        (501) staff       (20)      491 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/datastore/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7130 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/datastore/context.py
--rw-r--r--   0 jan        (501) staff       (20)     4761 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/datastore/remote.py
--rw-r--r--   0 jan        (501) staff       (20)    30290 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/datastore/simulator.py
--rw-r--r--   0 jan        (501) staff       (20)    11410 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/datastore/store.py
--rw-r--r--   0 jan        (501) staff       (20)    22669 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/device.py
--rw-r--r--   0 jan        (501) staff       (20)    30455 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/diag_message.py
--rw-r--r--   0 jan        (501) staff       (20)     6481 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/events.py
--rw-r--r--   0 jan        (501) staff       (20)     3206 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)    13673 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/factory.py
--rw-r--r--   0 jan        (501) staff       (20)    14708 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/file_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.400491 pymodbus-3.4.0/pymodbus/framer/
--rw-r--r--   0 jan        (501) staff       (20)      509 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/framer/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     5303 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/ascii_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     4448 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/base.py
--rw-r--r--   0 jan        (501) staff       (20)     6059 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/binary_framer.py
--rw-r--r--   0 jan        (501) staff       (20)    12255 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/rtu_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     6445 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/socket_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     4332 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/framer/tls_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     3921 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/logging.py
--rw-r--r--   0 jan        (501) staff       (20)     7745 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/mei_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15360 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/other_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15651 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/payload.py
--rw-r--r--   0 jan        (501) staff       (20)     7713 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/pdu.py
--rw-r--r--   0 jan        (501) staff       (20)        0 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/py.typed
--rw-r--r--   0 jan        (501) staff       (20)    14208 2023-07-20 12:10:38.000000 pymodbus-3.4.0/pymodbus/register_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)    12510 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/register_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.400598 pymodbus-3.4.0/pymodbus/repl/
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/repl/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.401157 pymodbus-3.4.0/pymodbus/repl/client/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/repl/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     5187 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/repl/client/completer.py
--rw-r--r--   0 jan        (501) staff       (20)     9526 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/repl/client/helper.py
--rw-r--r--   0 jan        (501) staff       (20)    13184 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/repl/client/main.py
--rw-r--r--   0 jan        (501) staff       (20)    23074 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/repl/client/mclient.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.401557 pymodbus-3.4.0/pymodbus/repl/server/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/repl/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     6912 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/repl/server/cli.py
--rw-r--r--   0 jan        (501) staff       (20)     6417 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/repl/server/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.401775 pymodbus-3.4.0/pymodbus/server/
--rw-r--r--   0 jan        (501) staff       (20)      996 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    29227 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/server/async_io.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.402138 pymodbus-3.4.0/pymodbus/server/reactive/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.4.0/pymodbus/server/reactive/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     1824 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/reactive/default_config.py
--rw-r--r--   0 jan        (501) staff       (20)    18653 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/reactive/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.402772 pymodbus-3.4.0/pymodbus/server/simulator/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/__init__.py
--rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/custom_actions.py
--rw-r--r--   0 jan        (501) staff       (20)    25319 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/simulator/http_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     4198 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/simulator/main.py
--rw-r--r--   0 jan        (501) staff       (20)     7619 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/server/simulator/setup.json
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.404024 pymodbus-3.4.0/pymodbus/server/simulator/web/
--rw-r--r--   0 jan        (501) staff       (20)    11369 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple120.png
--rw-r--r--   0 jan        (501) staff       (20)    15391 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple152.png
--rw-r--r--   0 jan        (501) staff       (20)     4817 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple60.png
--rw-r--r--   0 jan        (501) staff       (20)     6344 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/apple76.png
--rw-r--r--   0 jan        (501) staff       (20)    12014 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/favicon.ico
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.404773 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/
--rw-r--r--   0 jan        (501) staff       (20)     4314 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/calls
--rw-r--r--   0 jan        (501) staff       (20)     1132 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/log
--rw-r--r--   0 jan        (501) staff       (20)     5850 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
--rw-r--r--   0 jan        (501) staff       (20)     2710 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/registers
--rw-r--r--   0 jan        (501) staff       (20)      893 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/generator/server
--rw-r--r--   0 jan        (501) staff       (20)     1944 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/index.html
--rw-r--r--   0 jan        (501) staff       (20)      919 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/pymodbus.css
--rw-r--r--   0 jan        (501) staff       (20)      710 2023-07-19 18:58:37.000000 pymodbus-3.4.0/pymodbus/server/simulator/web/welcome.html
--rw-r--r--   0 jan        (501) staff       (20)    23600 2023-07-20 12:08:56.000000 pymodbus-3.4.0/pymodbus/transaction.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.405009 pymodbus-3.4.0/pymodbus/transport/
--rw-r--r--   0 jan        (501) staff       (20)       17 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/transport/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.405138 pymodbus-3.4.0/pymodbus/transport/serial_asyncio/
--rw-r--r--   0 jan        (501) staff       (20)    19336 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/transport/serial_asyncio/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    19112 2023-07-20 12:30:55.000000 pymodbus-3.4.0/pymodbus/transport/transport.py
--rw-r--r--   0 jan        (501) staff       (20)     7797 2023-07-20 10:02:40.000000 pymodbus-3.4.0/pymodbus/utilities.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.398200 pymodbus-3.4.0/pymodbus.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)    12723 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)     3402 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)      173 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/entry_points.txt
--rw-r--r--   0 jan        (501) staff       (20)      481 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/requires.txt
--rw-r--r--   0 jan        (501) staff       (20)        9 2023-07-20 12:31:08.000000 pymodbus-3.4.0/pymodbus.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.4.0/pymodbus.egg-info/zip-safe
--rw-r--r--   0 jan        (501) staff       (20)     1897 2023-07-20 12:08:56.000000 pymodbus-3.4.0/requirements.txt
--rw-r--r--   0 jan        (501) staff       (20)     4391 2023-07-20 12:31:08.409390 pymodbus-3.4.0/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)     1105 2023-07-20 10:02:40.000000 pymodbus-3.4.0/setup.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-20 12:31:08.408479 pymodbus-3.4.0/test/
--rw-r--r--   0 jan        (501) staff       (20)     3643 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_all_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     4594 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_bit_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5244 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_bit_write_messages.py
--rwxr-xr-x   0 jan        (501) staff       (20)    17813 2023-07-20 12:30:55.000000 pymodbus-3.4.0/test/test_client.py
--rw-r--r--   0 jan        (501) staff       (20)     1315 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_client_faulty_response.py
--rwxr-xr-x   0 jan        (501) staff       (20)    15957 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_client_sync.py
--rw-r--r--   0 jan        (501) staff       (20)    13200 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_device.py
--rw-r--r--   0 jan        (501) staff       (20)     8354 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_diag_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2359 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_events.py
--rw-r--r--   0 jan        (501) staff       (20)      771 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)     8499 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_factory.py
--rw-r--r--   0 jan        (501) staff       (20)    10180 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_file_message.py
--rw-r--r--   0 jan        (501) staff       (20)    11230 2023-07-20 12:30:55.000000 pymodbus-3.4.0/test/test_framers.py
--rw-r--r--   0 jan        (501) staff       (20)     1238 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_logging.py
--rw-r--r--   0 jan        (501) staff       (20)     6297 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_mei_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5687 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_other_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     8771 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_payload.py
--rw-r--r--   0 jan        (501) staff       (20)     2814 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_pdu.py
--rw-r--r--   0 jan        (501) staff       (20)     7450 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_register_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     7658 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_register_write_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2661 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_remote_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_repl_client.py
--rwxr-xr-x   0 jan        (501) staff       (20)    14440 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_server_asyncio.py
--rw-r--r--   0 jan        (501) staff       (20)     3546 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_server_context.py
--rw-r--r--   0 jan        (501) staff       (20)     8192 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_server_multidrop.py
--rw-r--r--   0 jan        (501) staff       (20)    23028 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_simulator.py
--rw-r--r--   0 jan        (501) staff       (20)      649 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_sparse_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)    31231 2023-07-20 12:08:56.000000 pymodbus-3.4.0/test/test_transaction.py
--rw-r--r--   0 jan        (501) staff       (20)     3107 2023-07-20 10:02:40.000000 pymodbus-3.4.0/test/test_utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.625681 pymodbus-3.4.1/
+-rw-r--r--   0 jan        (501) staff       (20)    29404 2023-07-27 14:55:12.000000 pymodbus-3.4.1/CHANGELOG.rst
+-rw-r--r--   0 jan        (501) staff       (20)     1392 2023-07-26 10:34:42.000000 pymodbus-3.4.1/LICENSE
+-rw-r--r--   0 jan        (501) staff       (20)       82 2023-07-26 10:34:42.000000 pymodbus-3.4.1/MANIFEST.in
+-rw-r--r--   0 jan        (501) staff       (20)    12545 2023-07-27 15:27:06.625784 pymodbus-3.4.1/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)    11051 2023-07-27 14:55:12.000000 pymodbus-3.4.1/README.rst
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.614724 pymodbus-3.4.1/pymodbus/
+-rw-r--r--   0 jan        (501) staff       (20)      316 2023-07-27 14:55:12.000000 pymodbus-3.4.1/pymodbus/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     9422 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/bit_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     9532 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/bit_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.616443 pymodbus-3.4.1/pymodbus/client/
+-rw-r--r--   0 jan        (501) staff       (20)      602 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    12296 2023-07-27 14:55:12.000000 pymodbus-3.4.1/pymodbus/client/base.py
+-rw-r--r--   0 jan        (501) staff       (20)    21046 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/client/mixin.py
+-rw-r--r--   0 jan        (501) staff       (20)     9723 2023-07-27 14:54:20.000000 pymodbus-3.4.1/pymodbus/client/serial.py
+-rw-r--r--   0 jan        (501) staff       (20)     9418 2023-07-27 14:55:12.000000 pymodbus-3.4.1/pymodbus/client/tcp.py
+-rw-r--r--   0 jan        (501) staff       (20)     5779 2023-07-27 14:54:20.000000 pymodbus-3.4.1/pymodbus/client/tls.py
+-rw-r--r--   0 jan        (501) staff       (20)     5629 2023-07-27 14:54:20.000000 pymodbus-3.4.1/pymodbus/client/udp.py
+-rw-r--r--   0 jan        (501) staff       (20)     3982 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/constants.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.617032 pymodbus-3.4.1/pymodbus/datastore/
+-rw-r--r--   0 jan        (501) staff       (20)      491 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/datastore/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7130 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/datastore/context.py
+-rw-r--r--   0 jan        (501) staff       (20)     4760 2023-07-27 14:55:12.000000 pymodbus-3.4.1/pymodbus/datastore/remote.py
+-rw-r--r--   0 jan        (501) staff       (20)    30290 2023-07-26 13:03:10.000000 pymodbus-3.4.1/pymodbus/datastore/simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)    11410 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/datastore/store.py
+-rw-r--r--   0 jan        (501) staff       (20)    22669 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/device.py
+-rw-r--r--   0 jan        (501) staff       (20)    30455 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/diag_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     6481 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/events.py
+-rw-r--r--   0 jan        (501) staff       (20)     3206 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)    13673 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    14708 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/file_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.617866 pymodbus-3.4.1/pymodbus/framer/
+-rw-r--r--   0 jan        (501) staff       (20)      509 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/framer/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     5303 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/framer/ascii_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     4448 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/framer/base.py
+-rw-r--r--   0 jan        (501) staff       (20)     6059 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/framer/binary_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)    12255 2023-07-26 12:02:54.000000 pymodbus-3.4.1/pymodbus/framer/rtu_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     6445 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/framer/socket_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     4332 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/framer/tls_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     3921 2023-07-26 13:03:10.000000 pymodbus-3.4.1/pymodbus/logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     7745 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/mei_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15360 2023-07-26 11:59:28.000000 pymodbus-3.4.1/pymodbus/other_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15651 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     7713 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)        0 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/py.typed
+-rw-r--r--   0 jan        (501) staff       (20)    14208 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/register_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    12510 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/register_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.617982 pymodbus-3.4.1/pymodbus/repl/
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.4.1/pymodbus/repl/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.618595 pymodbus-3.4.1/pymodbus/repl/client/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.4.1/pymodbus/repl/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     5187 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/repl/client/completer.py
+-rw-r--r--   0 jan        (501) staff       (20)     9528 2023-07-27 14:55:12.000000 pymodbus-3.4.1/pymodbus/repl/client/helper.py
+-rw-r--r--   0 jan        (501) staff       (20)    13184 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/repl/client/main.py
+-rw-r--r--   0 jan        (501) staff       (20)    23074 2023-07-26 12:02:54.000000 pymodbus-3.4.1/pymodbus/repl/client/mclient.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.618992 pymodbus-3.4.1/pymodbus/repl/server/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.4.1/pymodbus/repl/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     6912 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/repl/server/cli.py
+-rw-r--r--   0 jan        (501) staff       (20)     6417 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/repl/server/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.619234 pymodbus-3.4.1/pymodbus/server/
+-rw-r--r--   0 jan        (501) staff       (20)      996 2023-07-26 13:03:10.000000 pymodbus-3.4.1/pymodbus/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    29227 2023-07-27 14:54:20.000000 pymodbus-3.4.1/pymodbus/server/async_io.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.619575 pymodbus-3.4.1/pymodbus/server/reactive/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.4.1/pymodbus/server/reactive/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     1824 2023-07-26 11:14:14.000000 pymodbus-3.4.1/pymodbus/server/reactive/default_config.py
+-rw-r--r--   0 jan        (501) staff       (20)    18653 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/server/reactive/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.620289 pymodbus-3.4.1/pymodbus/server/simulator/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/__init__.py
+-rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/custom_actions.py
+-rw-r--r--   0 jan        (501) staff       (20)    25319 2023-07-26 13:03:10.000000 pymodbus-3.4.1/pymodbus/server/simulator/http_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     4198 2023-07-26 13:03:10.000000 pymodbus-3.4.1/pymodbus/server/simulator/main.py
+-rw-r--r--   0 jan        (501) staff       (20)     7619 2023-07-26 13:03:10.000000 pymodbus-3.4.1/pymodbus/server/simulator/setup.json
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.621291 pymodbus-3.4.1/pymodbus/server/simulator/web/
+-rw-r--r--   0 jan        (501) staff       (20)    11369 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/apple120.png
+-rw-r--r--   0 jan        (501) staff       (20)    15391 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/apple152.png
+-rw-r--r--   0 jan        (501) staff       (20)     4817 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/apple60.png
+-rw-r--r--   0 jan        (501) staff       (20)     6344 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/apple76.png
+-rw-r--r--   0 jan        (501) staff       (20)    12014 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/favicon.ico
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.621906 pymodbus-3.4.1/pymodbus/server/simulator/web/generator/
+-rw-r--r--   0 jan        (501) staff       (20)     4314 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/generator/calls
+-rw-r--r--   0 jan        (501) staff       (20)     1132 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/generator/log
+-rw-r--r--   0 jan        (501) staff       (20)     5850 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
+-rw-r--r--   0 jan        (501) staff       (20)     2710 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/generator/registers
+-rw-r--r--   0 jan        (501) staff       (20)      893 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/generator/server
+-rw-r--r--   0 jan        (501) staff       (20)     1944 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/index.html
+-rw-r--r--   0 jan        (501) staff       (20)      919 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/pymodbus.css
+-rw-r--r--   0 jan        (501) staff       (20)      710 2023-07-19 18:58:37.000000 pymodbus-3.4.1/pymodbus/server/simulator/web/welcome.html
+-rw-r--r--   0 jan        (501) staff       (20)    23600 2023-07-26 11:11:52.000000 pymodbus-3.4.1/pymodbus/transaction.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.622311 pymodbus-3.4.1/pymodbus/transport/
+-rw-r--r--   0 jan        (501) staff       (20)       17 2023-07-27 15:16:11.000000 pymodbus-3.4.1/pymodbus/transport/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    19450 2023-07-27 15:16:11.000000 pymodbus-3.4.1/pymodbus/transport/transport.py
+-rw-r--r--   0 jan        (501) staff       (20)     7770 2023-07-27 14:55:12.000000 pymodbus-3.4.1/pymodbus/transport/transport_serial.py
+-rw-r--r--   0 jan        (501) staff       (20)     7797 2023-07-26 10:34:42.000000 pymodbus-3.4.1/pymodbus/utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.615544 pymodbus-3.4.1/pymodbus.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)    12545 2023-07-27 15:27:06.000000 pymodbus-3.4.1/pymodbus.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)     3395 2023-07-27 15:27:06.000000 pymodbus-3.4.1/pymodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-27 15:27:06.000000 pymodbus-3.4.1/pymodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 jan        (501) staff       (20)      173 2023-07-27 15:27:06.000000 pymodbus-3.4.1/pymodbus.egg-info/entry_points.txt
+-rw-r--r--   0 jan        (501) staff       (20)      494 2023-07-27 15:27:06.000000 pymodbus-3.4.1/pymodbus.egg-info/requires.txt
+-rw-r--r--   0 jan        (501) staff       (20)        9 2023-07-27 15:27:06.000000 pymodbus-3.4.1/pymodbus.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.4.1/pymodbus.egg-info/zip-safe
+-rw-r--r--   0 jan        (501) staff       (20)     1910 2023-07-27 14:55:12.000000 pymodbus-3.4.1/requirements.txt
+-rw-r--r--   0 jan        (501) staff       (20)     4334 2023-07-27 15:27:06.626495 pymodbus-3.4.1/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)     1105 2023-07-26 10:34:42.000000 pymodbus-3.4.1/setup.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-27 15:27:06.625584 pymodbus-3.4.1/test/
+-rw-r--r--   0 jan        (501) staff       (20)     3643 2023-07-26 11:11:52.000000 pymodbus-3.4.1/test/test_all_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     4594 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_bit_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5244 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_bit_write_messages.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    17813 2023-07-27 15:16:11.000000 pymodbus-3.4.1/test/test_client.py
+-rw-r--r--   0 jan        (501) staff       (20)     1315 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_client_faulty_response.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    15954 2023-07-27 14:55:12.000000 pymodbus-3.4.1/test/test_client_sync.py
+-rw-r--r--   0 jan        (501) staff       (20)    13200 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_device.py
+-rw-r--r--   0 jan        (501) staff       (20)     8354 2023-07-26 11:59:28.000000 pymodbus-3.4.1/test/test_diag_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2359 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_events.py
+-rw-r--r--   0 jan        (501) staff       (20)      771 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)     8499 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    10180 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_file_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    11230 2023-07-27 15:16:11.000000 pymodbus-3.4.1/test/test_framers.py
+-rw-r--r--   0 jan        (501) staff       (20)     1238 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     6297 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_mei_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5687 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_other_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     8771 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     2814 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)     7450 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_register_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     7658 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_register_write_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2661 2023-07-26 11:11:52.000000 pymodbus-3.4.1/test/test_remote_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_repl_client.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    14440 2023-07-26 12:02:54.000000 pymodbus-3.4.1/test/test_server_asyncio.py
+-rw-r--r--   0 jan        (501) staff       (20)     3546 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_server_context.py
+-rw-r--r--   0 jan        (501) staff       (20)     8192 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_server_multidrop.py
+-rw-r--r--   0 jan        (501) staff       (20)    23028 2023-07-26 13:03:10.000000 pymodbus-3.4.1/test/test_simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)      649 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_sparse_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    31231 2023-07-26 11:59:28.000000 pymodbus-3.4.1/test/test_transaction.py
+-rw-r--r--   0 jan        (501) staff       (20)     3107 2023-07-26 10:34:42.000000 pymodbus-3.4.1/test/test_utilities.py
```

### Comparing `pymodbus-3.4.0/CHANGELOG.rst` & `pymodbus-3.4.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+version 3.4.1
+----------------------------------------------------------
+* Fix serial startup problems. (#1701)
+* pass source_address in tcp client. (#1700)
+* serial server use source_address[0]. (#1699)
+* Examples coverage nearly 100%. (#1694)
+* new async serial (#1681)
+* Docker is not supported (lack of maintainer). (#1693)
+* Forwarder write_coil --> write_coil. (#1691)
+* Change default source_address to (0.0.0.0, 502) (#1690)
+* Update ruff to 0.0.277 (#1689)
+* Fix dict comprehension (#1687)
+* Removed `requests` dependency from `contrib/explain.py`  (#1688)
+* Fix broken test (#1685)
+* Fix readme badges (#1682)
+* Bump aiohttp from 3.8.3 to 3.8.5 (#1680)
+* pygments from 2.14.0 to 2.15.0 (#1677)
+
+Thanks to:
+    Alex
+    James Braza
+    jan iversen
+
+
 version 3.4.0
 ----------------------------------------------------------
 * Prepare v3.4.0.
 * Handle partial local echo. (#1675)
 * clarify handle_local_echo. (#1674)
 * async_client: add retries/reconnect. (#1672)
 * Fix 3.11 problem. (#1673)
```

### Comparing `pymodbus-3.4.0/LICENSE` & `pymodbus-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/PKG-INFO` & `pymodbus-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.4.0
+Version: 3.4.1
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -41,31 +41,28 @@
 PyModbus - A Python Modbus Stack
 ================================
 We are constantly working the modernize pymodbus and add new features, and we look for people who want to help a bit.
 There are challenges small and large not only programming but also documentation and testing.
 
 .. image:: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml/badge.svg?branch=dev
    :target: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml
- .. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
+.. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
    :target: https://pymodbus.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
    :target: https://pepy.tech/project/pymodbus
    :alt: Downloads
-.. image:: https://ghcr-badge.deta.dev/pymodbus-dev/pymodbus/tags?label=Docker
-   :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
-   :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
 Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (python >= 2.7, no longer supported).
 
-Version `3.4.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.4.0>`_ is the current release (Tested with Python >= 3.8).
+Version `3.4.1 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.4.1>`_ is the current release (Tested with Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.4.0/README.rst` & `pymodbus-3.4.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 PyModbus - A Python Modbus Stack
 ================================
 We are constantly working the modernize pymodbus and add new features, and we look for people who want to help a bit.
 There are challenges small and large not only programming but also documentation and testing.
 
 .. image:: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml/badge.svg?branch=dev
    :target: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml
- .. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
+.. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
    :target: https://pymodbus.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
    :target: https://pepy.tech/project/pymodbus
    :alt: Downloads
-.. image:: https://ghcr-badge.deta.dev/pymodbus-dev/pymodbus/tags?label=Docker
-   :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
-   :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
 Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (python >= 2.7, no longer supported).
 
-Version `3.4.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.4.0>`_ is the current release (Tested with Python >= 3.8).
+Version `3.4.1 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.4.1>`_ is the current release (Tested with Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.4.0/pymodbus/bit_read_message.py` & `pymodbus-3.4.1/pymodbus/bit_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/bit_write_message.py` & `pymodbus-3.4.1/pymodbus/bit_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/client/__init__.py` & `pymodbus-3.4.1/pymodbus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/client/base.py` & `pymodbus-3.4.1/pymodbus/client/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     ) -> None:
         """Initialize a client instance."""
         ModbusClientMixin.__init__(self)
         self.use_sync = kwargs.get("use_sync", False)
         setup_params = CommParams(
             comm_type=kwargs.get("CommType"),
             comm_name="comm",
-            source_address=kwargs.get("source_address", ("127.0.0.1", 0)),
+            source_address=kwargs.get("source_address", ("0.0.0.0", 0)),
             reconnect_delay=reconnect_delay,
             reconnect_delay_max=reconnect_delay_max,
             timeout_connect=timeout,
             host=kwargs.get("host", None),
             port=kwargs.get("port", None),
             sslctx=kwargs.get("sslctx", None),
             baudrate=kwargs.get("baudrate", None),
@@ -172,18 +172,18 @@
 
         :param request: The request to process
         :returns: The result of the request execution
         :raises ConnectionException: Check exception text.
         """
         if self.use_sync:
             if not self.connected:
-                raise ConnectionException(f"Failed to connect[{str(self)}]")
+                raise ConnectionException(f"Failed to connect[{self!s}]")
             return self.transaction.execute(request)
         if not self.transport:
-            raise ConnectionException(f"Not connected[{str(self)}]")
+            raise ConnectionException(f"Not connected[{self!s}]")
         return self.async_execute(request)
 
     # ----------------------------------------------------------------------- #
     # Merged client methods
     # ----------------------------------------------------------------------- #
     async def async_execute(self, request=None):
         """Execute requests asynchronously."""
```

### Comparing `pymodbus-3.4.0/pymodbus/client/mixin.py` & `pymodbus-3.4.1/pymodbus/client/mixin.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/client/serial.py` & `pymodbus-3.4.1/pymodbus/client/serial.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/client/tcp.py` & `pymodbus-3.4.1/pymodbus/client/tcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         source_address: Tuple[str, int] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize Asyncio Modbus TCP Client."""
         asyncio.Protocol.__init__(self)
         if "CommType" not in kwargs:
             kwargs["CommType"] = CommType.TCP
+        if source_address:
+            kwargs["source_address"] = source_address
         ModbusBaseClient.__init__(
             self,
             framer=framer,
             host=host,
             port=port,
             **kwargs,
         )
```

### Comparing `pymodbus-3.4.0/pymodbus/client/tls.py` & `pymodbus-3.4.1/pymodbus/client/tls.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/client/udp.py` & `pymodbus-3.4.1/pymodbus/client/udp.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/constants.py` & `pymodbus-3.4.1/pymodbus/constants.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/datastore/context.py` & `pymodbus-3.4.1/pymodbus/datastore/context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/datastore/remote.py` & `pymodbus-3.4.1/pymodbus/datastore/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.__set_callbacks = {
             "d5": lambda a, v: self._client.write_coil(  # pylint: disable=unnecessary-lambda
                 a, v, **kwargs
             ),
             "d15": lambda a, v: self._client.write_coils(  # pylint: disable=unnecessary-lambda
                 a, v, **kwargs
             ),
-            "c5": lambda a, v: self._client.write_coils(  # pylint: disable=unnecessary-lambda
+            "c5": lambda a, v: self._client.write_coil(  # pylint: disable=unnecessary-lambda
                 a, v, **kwargs
             ),
             "c15": lambda a, v: self._client.write_coils(  # pylint: disable=unnecessary-lambda
                 a, v, **kwargs
             ),
             "h6": lambda a, v: self._client.write_register(  # pylint: disable=unnecessary-lambda
                 a, v, **kwargs
```

### Comparing `pymodbus-3.4.0/pymodbus/datastore/simulator.py` & `pymodbus-3.4.1/pymodbus/datastore/simulator.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/datastore/store.py` & `pymodbus-3.4.1/pymodbus/datastore/store.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/device.py` & `pymodbus-3.4.1/pymodbus/device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/diag_message.py` & `pymodbus-3.4.1/pymodbus/diag_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/events.py` & `pymodbus-3.4.1/pymodbus/events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/exceptions.py` & `pymodbus-3.4.1/pymodbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/factory.py` & `pymodbus-3.4.1/pymodbus/factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/file_message.py` & `pymodbus-3.4.1/pymodbus/file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/framer/ascii_framer.py` & `pymodbus-3.4.1/pymodbus/framer/ascii_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/framer/base.py` & `pymodbus-3.4.1/pymodbus/framer/base.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/framer/binary_framer.py` & `pymodbus-3.4.1/pymodbus/framer/binary_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/framer/rtu_framer.py` & `pymodbus-3.4.1/pymodbus/framer/rtu_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/framer/socket_framer.py` & `pymodbus-3.4.1/pymodbus/framer/socket_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/framer/tls_framer.py` & `pymodbus-3.4.1/pymodbus/framer/tls_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/logging.py` & `pymodbus-3.4.1/pymodbus/logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/mei_message.py` & `pymodbus-3.4.1/pymodbus/mei_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/other_message.py` & `pymodbus-3.4.1/pymodbus/other_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/payload.py` & `pymodbus-3.4.1/pymodbus/payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/pdu.py` & `pymodbus-3.4.1/pymodbus/pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/register_read_message.py` & `pymodbus-3.4.1/pymodbus/register_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/register_write_message.py` & `pymodbus-3.4.1/pymodbus/register_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/repl/client/completer.py` & `pymodbus-3.4.1/pymodbus/repl/client/completer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/repl/client/helper.py` & `pymodbus-3.4.1/pymodbus/repl/client/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,16 +175,16 @@
 
 def _get_client_methods(members):
     """Get client methods."""
     commands = list(
         filter(lambda x: (x[0] not in EXCLUDE and x[0] in CLIENT_METHODS), members)
     )
     commands = {
-        "client.{c[0]}": Command(
-            "client.{c[0]}", argspec(c[1]), inspect.getdoc(c[1]), slave=False
+        f"client.{c[0]}": Command(
+            f"client.{c[0]}", argspec(c[1]), inspect.getdoc(c[1]), slave=False
         )
         for c in commands
         if not c[0].startswith("_")
     }
     return commands
```

### Comparing `pymodbus-3.4.0/pymodbus/repl/client/main.py` & `pymodbus-3.4.1/pymodbus/repl/client/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/repl/client/mclient.py` & `pymodbus-3.4.1/pymodbus/repl/client/mclient.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/repl/server/cli.py` & `pymodbus-3.4.1/pymodbus/repl/server/cli.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/repl/server/main.py` & `pymodbus-3.4.1/pymodbus/repl/server/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/__init__.py` & `pymodbus-3.4.1/pymodbus/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/async_io.py` & `pymodbus-3.4.1/pymodbus/server/async_io.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/reactive/default_config.py` & `pymodbus-3.4.1/pymodbus/server/reactive/default_config.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/reactive/main.py` & `pymodbus-3.4.1/pymodbus/server/reactive/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/http_server.py` & `pymodbus-3.4.1/pymodbus/server/simulator/http_server.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/main.py` & `pymodbus-3.4.1/pymodbus/server/simulator/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/setup.json` & `pymodbus-3.4.1/pymodbus/server/simulator/setup.json`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/apple120.png` & `pymodbus-3.4.1/pymodbus/server/simulator/web/apple120.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/apple152.png` & `pymodbus-3.4.1/pymodbus/server/simulator/web/apple152.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/apple60.png` & `pymodbus-3.4.1/pymodbus/server/simulator/web/apple60.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/apple76.png` & `pymodbus-3.4.1/pymodbus/server/simulator/web/apple76.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/favicon.ico` & `pymodbus-3.4.1/pymodbus/server/simulator/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/calls` & `pymodbus-3.4.1/pymodbus/server/simulator/web/generator/calls`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/log` & `pymodbus-3.4.1/pymodbus/server/simulator/web/generator/log`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png` & `pymodbus-3.4.1/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/registers` & `pymodbus-3.4.1/pymodbus/server/simulator/web/generator/registers`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/generator/server` & `pymodbus-3.4.1/pymodbus/server/simulator/web/generator/server`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/index.html` & `pymodbus-3.4.1/pymodbus/server/simulator/web/index.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/pymodbus.css` & `pymodbus-3.4.1/pymodbus/server/simulator/web/pymodbus.css`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/server/simulator/web/welcome.html` & `pymodbus-3.4.1/pymodbus/server/simulator/web/welcome.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/transaction.py` & `pymodbus-3.4.1/pymodbus/transaction.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus/transport/transport.py` & `pymodbus-3.4.1/pymodbus/transport/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import asyncio
 import dataclasses
 import ssl
 from enum import Enum
 from typing import Any, Callable, Coroutine
 
 from pymodbus.logging import Log
-from pymodbus.transport.serial_asyncio import create_serial_connection
+from pymodbus.transport.transport_serial import create_serial_connection
 
 
 NULLMODEM_HOST = "__pymodbus_nullmodem"
 
 
 class CommType(Enum):
     """Type of transport"""
@@ -33,15 +33,15 @@
     comm_name: str = None
     comm_type: CommType = None
     reconnect_delay: float = None
     reconnect_delay_max: float = None
     timeout_connect: float = None
     host: str = "127.0.0.1"
     port: int = 0
-    source_address: tuple[str, int] = ("127.0.0.1", 0)
+    source_address: tuple[str, int] = ("0.0.0.0", 0)
     handle_local_echo: bool = False
 
     # tls
     sslctx: ssl.SSLContext = None
 
     # serial
     baudrate: int = None
@@ -169,18 +169,22 @@
 
         self.call_create = lambda: self.create_nullmodem(port)
         return True
 
     def init_setup_connect_listen(self) -> None:
         """Handle connect/listen handler."""
         if self.comm_params.comm_type == CommType.SERIAL:
+            if self.is_server:
+                host = self.comm_params.source_address[0]
+            else:
+                host = self.comm_params.host
             self.call_create = lambda: create_serial_connection(
                 self.loop,
                 self.handle_new_connection,
-                self.comm_params.host,
+                host,
                 baudrate=self.comm_params.baudrate,
                 bytesize=self.comm_params.bytesize,
                 parity=self.comm_params.parity,
                 stopbits=self.comm_params.stopbits,
                 timeout=self.comm_params.timeout_connect,
             )
             return
@@ -207,15 +211,15 @@
                 start_serving=True,
             )
         else:
             self.call_create = lambda: self.loop.create_connection(
                 self.handle_new_connection,
                 self.comm_params.host,
                 self.comm_params.port,
-                local_addr=self.comm_params.source_address,
+                # local_addr=self.comm_params.source_address,
                 ssl=self.comm_params.sslctx,
             )
 
     async def transport_connect(self) -> bool:
         """Handle generic connect and call on to specific transport connect."""
         Log.debug("Connecting {}", self.comm_params.comm_name)
         if not self.loop:
@@ -286,16 +290,14 @@
 
     def datagram_received(self, data: bytes, addr: tuple):
         """Receive datagram (UDP connections)."""
         if self.comm_params.handle_local_echo and self.sent_buffer:
             Log.debug("recv skipping (local_echo): {} addr={}", data, ":hex", addr)
             if self.sent_buffer in data:
                 data, self.sent_buffer = data.replace(self.sent_buffer, b"", 1), b""
-            elif self.sent_buffer.startswith(data):
-                self.sent_buffer, data = self.sent_buffer.replace(data, b"", 1), b""
             else:
                 self.sent_buffer = b""
             if not data:
                 return
         Log.debug("recv: {} addr={}", data, ":hex", addr)
         self.recv_buffer += data
         cut = self.callback_data(self.recv_buffer, addr=addr)
@@ -455,29 +457,29 @@
         self.transport_close()
 
     def __str__(self) -> str:
         """Build a string representation of the connection."""
         return f"{self.__class__.__name__}({self.comm_params.comm_name})"
 
 
-class NullModem(asyncio.DatagramTransport, asyncio.WriteTransport):
+class NullModem(asyncio.DatagramTransport, asyncio.Transport):
     """ModbusProtocol layer.
 
     Contains methods to act as a null modem between 2 objects.
     (Allowing tests to be shortcut without actual network calls)
     """
 
     listener_new_connection: dict[int, ModbusProtocol] = {}
 
     def __init__(self, protocol: ModbusProtocol):
         """Create half part of null modem"""
         asyncio.DatagramTransport.__init__(self)
-        asyncio.WriteTransport.__init__(self)
+        asyncio.Transport.__init__(self)
         self.other: NullModem = None
-        self.protocol = protocol
+        self.protocol: ModbusProtocol | asyncio.BaseProtocol = protocol
         self.serving: asyncio.Future = asyncio.Future()
         self.other_transport: NullModem = None
 
     # ---------------- #
     # external methods #
     # ---------------- #
 
@@ -504,18 +506,19 @@
         await self.serving
 
     # ---------------- #
     # Abstract methods #
     # ---------------- #
     def abort(self) -> None:
         """Abort connection."""
+        self.close()
 
     def can_write_eof(self) -> bool:
         """Allow to write eof"""
-        return True
+        return False
 
     def get_write_buffer_size(self) -> int:
         """Set write limit."""
         return 1024
 
     def get_write_buffer_limits(self) -> tuple[int, int]:
         """Set flush limits"""
@@ -523,17 +526,28 @@
 
     def set_write_buffer_limits(self, high: int = None, low: int = None) -> None:
         """Set flush limits"""
 
     def write_eof(self) -> None:
         """Write eof"""
 
-    def get_protocol(self) -> ModbusProtocol:
+    def get_protocol(self) -> ModbusProtocol | asyncio.BaseProtocol:
         """Return current protocol."""
-        return None
+        return self.protocol
 
     def set_protocol(self, protocol: asyncio.BaseProtocol) -> None:
         """Set current protocol."""
+        self.protocol = protocol
 
     def is_closing(self) -> bool:
         """Return true if closing"""
         return False
+
+    def is_reading(self) -> bool:
+        """Return true if read is active."""
+        return True
+
+    def pause_reading(self):
+        """Pause receiver."""
+
+    def resume_reading(self):
+        """Resume receiver."""
```

### Comparing `pymodbus-3.4.0/pymodbus/utilities.py` & `pymodbus-3.4.1/pymodbus/utilities.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/pymodbus.egg-info/PKG-INFO` & `pymodbus-3.4.1/pymodbus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.4.0
+Version: 3.4.1
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -41,31 +41,28 @@
 PyModbus - A Python Modbus Stack
 ================================
 We are constantly working the modernize pymodbus and add new features, and we look for people who want to help a bit.
 There are challenges small and large not only programming but also documentation and testing.
 
 .. image:: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml/badge.svg?branch=dev
    :target: https://github.com/pymodbus-dev/pymodbus/actions/workflows/ci.yml
- .. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
+.. image:: https://readthedocs.org/projects/pymodbus/badge/?version=latest
    :target: https://pymodbus.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://pepy.tech/badge/pymodbus
    :target: https://pepy.tech/project/pymodbus
    :alt: Downloads
-.. image:: https://ghcr-badge.deta.dev/pymodbus-dev/pymodbus/tags?label=Docker
-   :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
-   :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
 Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (python >= 2.7, no longer supported).
 
-Version `3.4.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.4.0>`_ is the current release (Tested with Python >= 3.8).
+Version `3.4.1 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.4.1>`_ is the current release (Tested with Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.4.0/pymodbus.egg-info/SOURCES.txt` & `pymodbus-3.4.1/pymodbus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 pymodbus/server/simulator/web/generator/calls
 pymodbus/server/simulator/web/generator/log
 pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
 pymodbus/server/simulator/web/generator/registers
 pymodbus/server/simulator/web/generator/server
 pymodbus/transport/__init__.py
 pymodbus/transport/transport.py
-pymodbus/transport/serial_asyncio/__init__.py
+pymodbus/transport/transport_serial.py
 test/test_all_messages.py
 test/test_bit_read_messages.py
 test/test_bit_write_messages.py
 test/test_client.py
 test/test_client_faulty_response.py
 test/test_client_sync.py
 test/test_device.py
```

### Comparing `pymodbus-3.4.0/requirements.txt` & `pymodbus-3.4.1/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,46 +19,47 @@
 # These packages are optional for the runtime, but demanded for
 # document generation, development and test.
 #
 # these packages can be installed like:
 #    pip install pymodbus[serial]
 
 # install:repl
-aiohttp==3.8.3
-typer[all]==0.7.0
-prompt-toolkit==3.0.36
-pygments==2.14.0
+aiohttp>=3.8.5
+typer[all]>=0.7.0
+prompt-toolkit>=3.0.36
+pygments>=2.15.0
 click>=8.0.0
 
 # install:serial
 pyserial>=3.5
 
 
 # -------------------------------------------------------------------
 # documentation, everything needed to generate documentation.
 # -------------------------------------------------------------------
 # install:documentation
-recommonmark==0.7.1
-Sphinx==5.3.0
-sphinx-rtd-theme==1.1.1
+recommonmark>=0.7.1
+Sphinx>=5.3.0
+sphinx-rtd-theme>=1.1.1
 
 
 # -------------------------------------------------------------------
 # development, everything needed to develop/test/check.
 # -------------------------------------------------------------------
 # install:development
-codespell==2.2.2
-coverage==7.1.0
-mypy==1.3.0
-pre-commit==3.1.1
-pyflakes==3.0.1
-pydocstyle==6.3.0
-pycodestyle==2.10.0
-pylint==2.17.2
-pytest==7.3.1
-pytest-asyncio==0.20.3
-pytest-cov==4.1.0
-pytest-timeout==2.1.0
-pytest-xdist==3.3.1
-ruff==0.0.261
+codespell>=2.2.2
+coverage>=7.1.0
+mypy>=1.3.0
+pre-commit>=3.1.1
+pyflakes>=3.0.1
+pydocstyle>=6.3.0
+pycodestyle>=2.10.0
+pylint>=2.17.2
+pytest>=7.3.1
+pytest-asyncio>=0.20.3
+pytest-cov>=4.1.0
+pytest-timeout>=2.1.0
+pytest-xdist>=3.3.1
+ruff>=0.0.277
 types-Pygments
 types-pyserial
+twine>=4.0.2
```

### Comparing `pymodbus-3.4.0/setup.cfg` & `pymodbus-3.4.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -166,18 +166,17 @@
 testpaths = test
 addopts = -p no:warnings --dist loadgroup --numprocesses auto
 asyncio_mode = auto
 timeout = 40
 
 [coverage:run]
 include = 
+	examples/
 	pymodbus/
 	test/
 omit = 
-	test/TO_DO_REWRITE
-	examples/common/tornado_twister
-	examples/contrib/tornado_twister
+	examples/contrib/
 
 [codespell]
 skip = ./doc/_build,./doc/source/_static,venv,.venv,.git,htmlcov,CHANGELOG.rst,.mypy_cache
 ignore-words-list = asend
```

### Comparing `pymodbus-3.4.0/setup.py` & `pymodbus-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_all_messages.py` & `pymodbus-3.4.1/test/test_all_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_bit_read_messages.py` & `pymodbus-3.4.1/test/test_bit_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_bit_write_messages.py` & `pymodbus-3.4.1/test/test_bit_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_client.py` & `pymodbus-3.4.1/test/test_client.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_client_faulty_response.py` & `pymodbus-3.4.1/test/test_client_faulty_response.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_client_sync.py` & `pymodbus-3.4.1/test/test_client_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             """Dummy custom request."""
 
             function_code = 79
 
         client = ModbusTcpClient("127.0.0.1")
         client.framer = mock.Mock()
         client.register(CustomRequest)
-        assert client.framer.decoder.register.called_once_with(CustomRequest)
+        client.framer.decoder.register.assert_called_once_with(CustomRequest)
 
     # -----------------------------------------------------------------------#
     # Test TLS Client
     # -----------------------------------------------------------------------#
 
     def test_syn_tls_client_instantiation(self):
         """Test sync tls client."""
@@ -277,23 +277,23 @@
             f"timeout={client.comm_params.timeout_connect}>"
         )
         assert repr(client) == rep
 
     def test_tls_client_register(self):
         """Test tls client."""
 
-        class CustomeRequest:  # pylint: disable=too-few-public-methods
+        class CustomRequest:  # pylint: disable=too-few-public-methods
             """Dummy custom request."""
 
             function_code = 79
 
         client = ModbusTlsClient("127.0.0.1")
         client.framer = mock.Mock()
-        client.register(CustomeRequest)
-        assert client.framer.decoder.register.called_once_with(CustomeRequest)
+        client.register(CustomRequest)
+        client.framer.decoder.register.assert_called_once_with(CustomRequest)
 
     # -----------------------------------------------------------------------#
     # Test Serial Client
     # -----------------------------------------------------------------------#
     def test_sync_serial_client_instantiation(self):
         """Test sync serial client."""
         client = ModbusSerialClient("/dev/null")
```

### Comparing `pymodbus-3.4.0/test/test_device.py` & `pymodbus-3.4.1/test/test_device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_diag_messages.py` & `pymodbus-3.4.1/test/test_diag_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_events.py` & `pymodbus-3.4.1/test/test_events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_exceptions.py` & `pymodbus-3.4.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_factory.py` & `pymodbus-3.4.1/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_file_message.py` & `pymodbus-3.4.1/test/test_file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_framers.py` & `pymodbus-3.4.1/test/test_framers.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_logging.py` & `pymodbus-3.4.1/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_mei_messages.py` & `pymodbus-3.4.1/test/test_mei_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_other_messages.py` & `pymodbus-3.4.1/test/test_other_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_payload.py` & `pymodbus-3.4.1/test/test_payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_pdu.py` & `pymodbus-3.4.1/test/test_pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_register_read_messages.py` & `pymodbus-3.4.1/test/test_register_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_register_write_messages.py` & `pymodbus-3.4.1/test/test_register_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_remote_datastore.py` & `pymodbus-3.4.1/test/test_remote_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_repl_client.py` & `pymodbus-3.4.1/test/test_repl_client.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_server_asyncio.py` & `pymodbus-3.4.1/test/test_server_asyncio.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_server_context.py` & `pymodbus-3.4.1/test/test_server_context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_server_multidrop.py` & `pymodbus-3.4.1/test/test_server_multidrop.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_simulator.py` & `pymodbus-3.4.1/test/test_simulator.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_sparse_datastore.py` & `pymodbus-3.4.1/test/test_sparse_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_transaction.py` & `pymodbus-3.4.1/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.4.0/test/test_utilities.py` & `pymodbus-3.4.1/test/test_utilities.py`

 * *Files identical despite different names*

