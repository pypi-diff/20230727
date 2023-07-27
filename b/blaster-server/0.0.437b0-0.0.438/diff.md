# Comparing `tmp/blaster-server-0.0.437b0.tar.gz` & `tmp/blaster-server-0.0.438.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.437b0.tar", last modified: Sun Jun 25 09:53:32 2023, max compression
+gzip compressed data, was "blaster-server-0.0.438.tar", last modified: Thu Jul 27 00:08:03 2023, max compression
```

## Comparing `blaster-server-0.0.437b0.tar` & `blaster-server-0.0.438.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.437b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.437b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.437b0/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.437b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    61703 2023-06-23 10:38:33.000000 blaster-server-0.0.437b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15679 2023-06-07 13:51:59.000000 blaster-server-0.0.437b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38833 2023-06-09 14:07:27.000000 blaster-server-0.0.437b0/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    43733 2023-06-24 12:52:51.000000 blaster-server-0.0.437b0/blaster/tools/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.437b0/blaster/tools/sanitize_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3950 2023-06-13 13:22:35.000000 blaster-server-0.0.437b0/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.978733 blaster-server-0.0.437b0/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-25 09:53:32.000000 blaster-server-0.0.437b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1741 2023-06-23 10:38:41.000000 blaster-server-0.0.437b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-06-17 08:57:19.000000 blaster-server-0.0.437b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-25 09:53:32.982733 blaster-server-0.0.437b0/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.437b0/test/test_command_line_parser.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.437b0/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.437b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.437b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.667643 blaster-server-0.0.438/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.438/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.438/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-07-27 00:08:03.667643 blaster-server-0.0.438/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.438/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.663643 blaster-server-0.0.438/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.438/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.663643 blaster-server-0.0.438/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.438/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.663643 blaster-server-0.0.438/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.438/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.438/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.438/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.438/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.438/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    61703 2023-07-19 07:59:01.000000 blaster-server-0.0.438/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15799 2023-07-27 00:06:27.000000 blaster-server-0.0.438/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38638 2023-07-27 00:05:21.000000 blaster-server-0.0.438/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.663643 blaster-server-0.0.438/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    43733 2023-07-19 07:59:08.000000 blaster-server-0.0.438/blaster/tools/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.438/blaster/tools/sanitize_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.663643 blaster-server-0.0.438/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.663643 blaster-server-0.0.438/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.438/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3950 2023-06-13 13:22:35.000000 blaster-server-0.0.438/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.667643 blaster-server-0.0.438/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.667643 blaster-server-0.0.438/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.438/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.667643 blaster-server-0.0.438/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-07-27 00:08:03.000000 blaster-server-0.0.438/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-07-27 00:08:03.000000 blaster-server-0.0.438/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-07-27 00:08:03.000000 blaster-server-0.0.438/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-07-27 00:08:03.000000 blaster-server-0.0.438/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-07-27 00:08:03.000000 blaster-server-0.0.438/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.667643 blaster-server-0.0.438/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1741 2023-06-23 10:38:41.000000 blaster-server-0.0.438/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.438/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-07-27 00:08:03.667643 blaster-server-0.0.438/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-07-27 00:03:57.000000 blaster-server-0.0.438/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 00:08:03.667643 blaster-server-0.0.438/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.438/test/test_command_line_parser.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.438/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.438/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.438/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.438/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.438/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.438/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.437b0/LICENSE.txt` & `blaster-server-0.0.438/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/PKG-INFO` & `blaster-server-0.0.438/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.437b0
+Version: 0.0.438
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.437b0/README.md` & `blaster-server-0.0.438/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/__init__.py` & `blaster-server-0.0.438/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/cloud/analytics.py` & `blaster-server-0.0.438/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.438/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.438/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/cloud/storage.py` & `blaster-server-0.0.438/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/config.py` & `blaster-server-0.0.438/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/connection_pool.py` & `blaster-server-0.0.438/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/env.py` & `blaster-server-0.0.438/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/logging.py` & `blaster-server-0.0.438/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/mongo_orm.py` & `blaster-server-0.0.438/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/schema.py` & `blaster-server-0.0.438/blaster/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 			if(self._default != _OBJ_END_):
 				return self._default
 			raise TypeError("should be int")
 		if(isinstance(e, str) and len(e) > 50):
 			raise TypeError("should be valid int")
 		e = self._type(e)
 		if(self._min != _OBJ_END_ and e < self._min):
-			raise TypeError("should be minlen {:d}".format(self._min))
+			raise TypeError("should be min {:d}".format(self._min))
 		if(self._max != _OBJ_END_ and e > self._max):
-			raise TypeError("more than maxlen {:d}".format(self._max))
+			raise TypeError("more than max {:d}".format(self._max))
 		if(self.one_of and e not in self.one_of):
 			raise TypeError("should be one of {:d}".format(str(self.one_of)))
 		return e
 
 
 class Int(Number):
 	def __init__(self, *args, **kwargs):
@@ -84,14 +84,15 @@
 		super().__init__(*args, _type=float, **kwargs)
 
 
 class Bool:
 	def __init__(self, default=_OBJ_END_, _name=None):
 		self._schema_ = _schema = {"type": "boolean"}
 		self._name = _name
+		self._default = default
 		if(default != _OBJ_END_):
 			_schema["default"] = default
 
 	def validate(self, e):
 		if(e == None):
 			if(self._default != _OBJ_END_):
 				return self._default
@@ -193,15 +194,15 @@
 		)
 
 	def __getitem__(self, *keys):
 		return Array(keys)
 
 
 # Type definitions:
-# - Object 
+# - Object
 #  {"a": b, 1: 2...}
 
 # - Object(Str, Str)
 #  {"a": "1", "b": "2"...}
 
 # - Object(Str, Optional[Int, Str])
 #  {"a": "1", "b": "2"...}
@@ -374,15 +375,18 @@
 			# None or copy of default
 			return list(_type._default) if _type._default != None else None
 		if(nullable):
 			return None
 		raise TypeError("Cannot be none")
 
 	if(not isinstance(arr, list)):
-		arr = json.loads(arr)
+		if(isinstance(arr, str) and arr.startswith("[")):
+			arr = json.loads(arr)
+		else:
+			raise TypeError("Not an array type")
 
 	_prev_type = _OBJ_END_
 	for i in range(len(arr)):
 		e = item_validation(arr[i], simple_types, complex_validations, nullable)
 		# check types should not mixed
 		if(not mix):  # single type, so check type matches with previous
 			_cur_type = type(e)
```

### Comparing `blaster-server-0.0.437b0/blaster/server.py` & `blaster-server-0.0.438/blaster/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from . import req_ctx
 from .tools import set_socket_fast_close_options,\
 	BufferedSocket, ltrim, _OBJ_END_
 from .tools.sanitize_html import SanitizedDict
 from .utils import events
 from .utils.data_utils import FILE_EXTENSION_TO_MIME_TYPE
 from .logging import LOG_ERROR, LOG_SERVER, LOG_WARN, LOG_DEBUG
-from .schema import Int, Object, Required, schema as schema_func
+from .schema import Object, Required, schema as schema_func
 from .websocket.server import WebSocketServerHandler
 from .config import IS_DEV, BLASTER_HTTP_TOOK_LONG_WARN_THRESHOLD
 
 if(IS_DEV):
 	# dev specific config
 	from .config import DEV_FORCE_ACCESS_CONTROL_ALLOW_ORIGIN
 
@@ -339,44 +339,36 @@
 			if(ret != None):
 				return ret
 			elif(default != _OBJ_END_):
 				return default
 			raise MissingBlasterArgumentException(name, _type)
 		return wrapper
 
-	# create the value of the argument based on type, default
 	@classmethod
 	def arg_generator(cls, name, _type, default):
-		if(_type in (str, int, float)):
-			return lambda req: (_type(_val) if _val != None else None)\
-				if (_val := req.get(name, default)) != _OBJ_END_\
-				else raise_ex(
-					MissingBlasterArgumentException(name, _type)
-			)
-		elif(_type == Request):  # req: Request
+		'''
+			This should PREPROCESS as much as possible and return a function 
+			that create the argument from the request
+		'''
+		if(_type == Request):  # req: Request
 			return lambda req: req
 		elif(_type == Query):  # query: Query
 			return lambda req: req._params
 		elif(_type == Headers):  # headers: Headers
 			return lambda req: req._headers
 		elif(_type == Body):  # headers: Headers
 			return lambda req: req._body
-		elif(isinstance(_type, (Int, str))):
-			return lambda req: _type.validate(req.get(name), default=default)
 		elif(isinstance(_type, Query)):  # Query(id=str, abc=str)
 			return lambda req: _type.from_dict(req._params, default=default)
-
 		elif(isinstance(_type, Headers)):  # Headers('user-agent')
 			return lambda req: _type.from_dict(req._headers, default=default)
-
 		elif(isinstance(_type, Body)):
 			return lambda req: _type.from_dict(req._body, default=default)
 
-		# type should be class at this point
-		# if has an arg injector, use it
+		# prefer arg injector first if available
 		has_arg_creator_hook = _argument_creator_hooks.get(_type)
 		if(has_arg_creator_hook):
 			return Request.wrap_arg_hook_for_defaults(has_arg_creator_hook, name, _type, default)
 
 		elif(isinstance(_type, type) and issubclass(_type, Body)):
 			return lambda req: _type.from_dict(req._body, default=default)
 
@@ -386,22 +378,24 @@
 		elif(
 			isinstance(_type, Object)
 			or (isinstance(_type, type) and issubclass(_type, Object))
 		):
 			return lambda req: _type.from_dict(req, default=default)
 
 		else:
+			_, validate = schema_func(_type, _default=default)
+
 			def _no_type_arg(req):
 				ret = req.get(name, default=_OBJ_END_)
 				if(ret == _OBJ_END_):
 					if(default == _OBJ_END_):
 						# Unknown field type
 						raise TypeError("{:s} field is required".format(name))
 					return default
-				return ret
+				return validate(ret)
 			return _no_type_arg
 
 	def to_dict(self):
 		return {"get": self._params, "post": self._body}
 
 
 # contains all running apps
@@ -790,14 +784,15 @@
 		resuse_socket_for_next_http_request = True
 		# ignore request lines > 4096 bytes
 		request_line = buffered_socket.readuntil('\r\n', 4096, True)
 		if(not request_line):
 			return
 		post_data = None
 		req = req_ctx.req = Request(buffered_socket, req_ctx)
+		# set all usable timestamp variables at once
 		cur_millis \
 			= req_ctx.timestamp \
 			= req.timestamp \
 			= int(1000 * time.time())
 		request_type = None
 		request_path = None
 		headers = None
@@ -1036,15 +1031,15 @@
 				_wallclock_ms = int(1000 * time.time()) - cur_millis
 				LOG_SERVER(
 					"http", response_status=status, request_type=request_type,
 					path=request_path, content_length=content_length,
 					wallclockms=_wallclock_ms
 				)
 				if(_wallclock_ms > BLASTER_HTTP_TOOK_LONG_WARN_THRESHOLD):
-					LOG_ERROR(
+					LOG_WARN(
 						"http_took_long", response_status=status, request_type=request_type,
 						path=request_path, content_length=content_length,
 						body_len=req._body_raw and len(req._body_raw),
 						req_str=str(req.to_dict())[:16 * _1_KB_],
 						wallclockms=_wallclock_ms
 					)
```

### Comparing `blaster-server-0.0.437b0/blaster/tools/__init__.py` & `blaster-server-0.0.438/blaster/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/tools/sanitize_html.py` & `blaster-server-0.0.438/blaster/tools/sanitize_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/data/countries.json` & `blaster-server-0.0.438/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.438/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/data_utils.py` & `blaster-server-0.0.438/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/events.py` & `blaster-server-0.0.438/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/fork.py` & `blaster-server-0.0.438/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.438/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.438/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/utils/xss_html.py` & `blaster-server-0.0.438/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/__init__.py` & `blaster-server-0.0.438/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.438/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_app.py` & `blaster-server-0.0.438/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_core.py` & `blaster-server-0.0.438/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.438/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.438/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_http.py` & `blaster-server-0.0.438/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_logging.py` & `blaster-server-0.0.438/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_socket.py` & `blaster-server-0.0.438/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.438/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_url.py` & `blaster-server-0.0.438/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/_utils.py` & `blaster-server-0.0.438/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/server.py` & `blaster-server-0.0.438/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.438/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.438/blaster_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.437b0
+Version: 0.0.438
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.437b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.438/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.438/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/examples/mongo_ormexample.py` & `blaster-server-0.0.438/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/examples/simple_examples.py` & `blaster-server-0.0.438/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/examples/test_chat_room.py` & `blaster-server-0.0.438/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/examples/tornado_hello_world.py` & `blaster-server-0.0.438/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/examples/wheezy_hello.py` & `blaster-server-0.0.438/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/setup.py` & `blaster-server-0.0.438/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.437b',
+	version='0.0.438',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.437b0/test/test_mongo_orm.py` & `blaster-server-0.0.438/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/test/test_phone_number_utils.py` & `blaster-server-0.0.438/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/test/test_schema.py` & `blaster-server-0.0.438/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/test/test_tools.py` & `blaster-server-0.0.438/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/test/test_utils.py` & `blaster-server-0.0.438/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.437b0/test/timeit_snippets.py` & `blaster-server-0.0.438/test/timeit_snippets.py`

 * *Files identical despite different names*

