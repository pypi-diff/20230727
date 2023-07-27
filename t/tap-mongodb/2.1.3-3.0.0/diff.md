# Comparing `tmp/tap-mongodb-2.1.3.tar.gz` & `tmp/tap-mongodb-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mongodb-2.1.3.tar", last modified: Tue Jul 25 19:32:34 2023, max compression
+gzip compressed data, was "tap-mongodb-3.0.0.tar", last modified: Thu Jul 27 19:13:13 2023, max compression
```

## Comparing `tap-mongodb-2.1.3.tar` & `tap-mongodb-3.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32386 2023-04-20 13:58:35.000000 tap-mongodb-2.1.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3667 2023-04-20 13:58:35.000000 tap-mongodb-2.1.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      782 2023-07-25 19:32:02.000000 tap-mongodb-2.1.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.236862 tap-mongodb-2.1.3/tap_mongodb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14726 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tap_mongodb/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.240862 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13349 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6988 2023-07-25 18:29:25.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/full_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5170 2023-04-20 13:58:35.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/incremental.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10900 2023-07-25 17:28:52.000000 tap-mongodb-2.1.3/tap_mongodb/sync_strategies/oplog.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.236862 tap-mongodb-2.1.3/tap_mongodb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1253 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-07-25 19:32:34.000000 tap-mongodb-2.1.3/tap_mongodb.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:32:34.252862 tap-mongodb-2.1.3/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11331 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_cname_restrictions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6918 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_configurable_properties.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10014 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_datatype.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11497 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13941 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_fname_restrictions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12712 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_full_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10542 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_full_table_id.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10412 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_full_table_interruptible.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10648 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_id_pk_variations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25133 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_incremental.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13090 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_incremental_open_transactions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6285 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_index.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14615 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_log_based_interruptible.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12493 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_name_restrictions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11531 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_namespace_restrictions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11077 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_oplog.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_oplog_aged_out.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9714 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_oplog_bookmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9763 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_projection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12817 2023-07-25 18:29:15.000000 tap-mongodb-2.1.3/tests/test_mongodb_table_reset_inc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8070 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_table_reset_log.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5635 2023-07-24 18:36:58.000000 tap-mongodb-2.1.3/tests/test_mongodb_views.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 19:13:13.022138 tap-mongodb-3.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32386 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-27 19:13:13.022138 tap-mongodb-3.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3667 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-27 19:13:13.022138 tap-mongodb-3.0.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      781 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 19:13:13.014138 tap-mongodb-3.0.0/tap_mongodb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14886 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tap_mongodb/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 19:13:13.018138 tap-mongodb-3.0.0/tap_mongodb/sync_strategies/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14170 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tap_mongodb/sync_strategies/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6988 2023-07-26 12:10:24.000000 tap-mongodb-3.0.0/tap_mongodb/sync_strategies/full_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5170 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tap_mongodb/sync_strategies/incremental.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10900 2023-07-26 12:12:12.000000 tap-mongodb-3.0.0/tap_mongodb/sync_strategies/oplog.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 19:13:13.018138 tap-mongodb-3.0.0/tap_mongodb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-07-27 19:13:12.000000 tap-mongodb-3.0.0/tap_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1253 2023-07-27 19:13:12.000000 tap-mongodb-3.0.0/tap_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 19:13:12.000000 tap-mongodb-3.0.0/tap_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-27 19:13:12.000000 tap-mongodb-3.0.0/tap_mongodb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2023-07-27 19:13:12.000000 tap-mongodb-3.0.0/tap_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-07-27 19:13:12.000000 tap-mongodb-3.0.0/tap_mongodb.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 19:13:13.022138 tap-mongodb-3.0.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11331 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_cname_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6918 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_configurable_properties.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10544 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tests/test_mongodb_datatype.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11497 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14057 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tests/test_mongodb_fname_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12712 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_full_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10542 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_full_table_id.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10412 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_full_table_interruptible.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10648 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_id_pk_variations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25201 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tests/test_mongodb_incremental.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14765 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tests/test_mongodb_incremental_open_transactions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6285 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14615 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_log_based_interruptible.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12505 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tests/test_mongodb_name_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11531 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_namespace_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11077 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_oplog.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_oplog_aged_out.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9714 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_oplog_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10154 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tests/test_mongodb_projection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12827 2023-07-27 19:11:54.000000 tap-mongodb-3.0.0/tests/test_mongodb_table_reset_inc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8070 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_table_reset_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5635 2023-06-29 12:22:41.000000 tap-mongodb-3.0.0/tests/test_mongodb_views.py
```

### Comparing `tap-mongodb-2.1.3/LICENSE` & `tap-mongodb-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/README.md` & `tap-mongodb-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/setup.py` & `tap-mongodb-3.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-mongodb',
-      version='2.1.3',
+      version='3.0.0',
       description='Singer.io tap for extracting data from MongoDB',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mongodb'],
       install_requires=[
           'singer-python==5.8.0',
-          'pymongo==3.12.3',
+          'pymongo==4.4.0',
           'tzlocal==2.0.0',
           'terminaltables==3.1.0',
       ],
       extras_require={
           'dev': [
               'pylint',
               'nose',
```

### Comparing `tap-mongodb-2.1.3/tap_mongodb/__init__.py` & `tap-mongodb-3.0.0/tap_mongodb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import copy
 import json
 import ssl
 import sys
 import time
 import pymongo
-from bson import timestamp
+from bson.codec_options import DatetimeConversion
 
 import singer
 from singer import metadata, metrics, utils
 
 import tap_mongodb.sync_strategies.common as common
 import tap_mongodb.sync_strategies.full_table as full_table
 import tap_mongodb.sync_strategies.oplog as oplog
@@ -229,15 +229,18 @@
         stream=common.calculate_destination_stream_name(stream),
         schema=stream['schema'],
         key_properties=['_id']))
 
 def load_stream_projection(stream):
     md_map = metadata.to_map(stream['metadata'])
     stream_projection = metadata.get(md_map, (), 'tap-mongodb.projection')
-    if stream_projection == '' or stream_projection == '""' or not stream_projection:
+    if (stream_projection == ''
+        or stream_projection == '""'
+        or stream_projection == '{}'
+        or not stream_projection):
         return None
 
     try:
         stream_projection = json.loads(stream_projection)
     except Exception as ex:
         err_msg = "The projection: {} for stream {} is not valid json"
         raise common.InvalidProjectionException(err_msg.format(stream_projection,
@@ -362,15 +365,16 @@
     connection_params = {"host": config['host'],
                          "port": int(config['port']),
                          "username": config.get('user', None),
                          "password": config.get('password', None),
                          "authSource": config['database'],
                          "ssl": use_ssl,
                          "replicaset": config.get('replica_set', None),
-                         "readPreference": 'secondaryPreferred'}
+                         "readPreference": 'secondaryPreferred',
+                         "datetime_conversion": DatetimeConversion.DATETIME_AUTO}
 
     # NB: "ssl_cert_reqs" must ONLY be supplied if `SSL` is true.
     if not verify_mode and use_ssl:
         connection_params["ssl_cert_reqs"] = ssl.CERT_NONE
 
     client = pymongo.MongoClient(**connection_params)
```

### Comparing `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/common.py` & `tap-mongodb-3.0.0/tap_mongodb/sync_strategies/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/env python3
 import base64
 import datetime
 import time
 import uuid
 import decimal
 import bson
-from bson import objectid, timestamp, datetime as bson_datetime
 import singer
 from singer import utils, metadata
 from terminaltables import AsciiTable
+from bson import objectid, timestamp, encode, decode, datetime as bson_datetime
+from bson.binary import Binary, UuidRepresentation
+from bson.codec_options import CodecOptions, DatetimeConversion
+from bson.datetime_ms import DatetimeMS
 
 import pytz
 import tzlocal
 
 INCLUDE_SCHEMAS_IN_DESTINATION_STREAM_NAME = False
 UPDATE_BOOKMARK_PERIOD = 1000
 COUNTS = {}
@@ -63,14 +66,17 @@
         return utils.strftime(utc_datetime)
     if bookmark_type == 'Timestamp':
         return '{}.{}'.format(bookmark_value.time, bookmark_value.inc)
     if bookmark_type == 'bytes':
         return base64.b64encode(bookmark_value).decode('utf-8')
     if bookmark_type in ['int', 'Int64', 'float', 'ObjectId', 'str', 'UUID']:
         return str(bookmark_value)
+    if bookmark_type == 'Binary':
+        return str(bookmark_value.as_uuid(bookmark_value.subtype))
+
     raise UnsupportedReplicationKeyTypeException("{} is not a supported replication key type"
                                                  .format(bookmark_type))
 
 
 # pylint: disable=too-many-return-statements
 def string_to_class(str_value, type_value):
     if type_value == 'UUID':
@@ -88,14 +94,16 @@
     if type_value == 'Timestamp':
         split_value = str_value.split('.')
         return bson.timestamp.Timestamp(int(split_value[0]), int(split_value[1]))
     if type_value == 'bytes':
         return base64.b64decode(str_value.encode())
     if type_value == 'str':
         return str(str_value)
+    if type_value == 'Binary':
+        return Binary.from_uuid(uuid.UUID(str_value), UuidRepresentation.STANDARD)
     raise UnsupportedReplicationKeyTypeException("{} is not a supported replication key type"
                                                  .format(type_value))
 
 def safe_transform_datetime(value, path):
     timezone = tzlocal.get_localzone()
     try:
         local_datetime = timezone.localize(value)
@@ -131,14 +139,16 @@
         return str(value)
     if isinstance(value, bson_datetime.datetime):
         return safe_transform_datetime(value, path)
     if isinstance(value, timestamp.Timestamp):
         return utils.strftime(value.as_datetime())
     if isinstance(value, bson.int64.Int64):
         return int(value)
+    if isinstance(value, Binary):
+        return str(value.as_uuid(value.subtype))
     if isinstance(value, bytes):
         # Return the original base64 encoded string
         return base64.b64encode(value).decode('utf-8')
     if isinstance(value, datetime.datetime):
         timezone = tzlocal.get_localzone()
         local_datetime = timezone.localize(value)
         utc_datetime = local_datetime.astimezone(pytz.UTC)
@@ -159,14 +169,19 @@
         }
     if isinstance(value, bson.dbref.DBRef):
         return {
             'id': str(value.id),
             'collection': value.collection,
             'database': value.database
         }
+    if isinstance(value, DatetimeMS):
+        encoded_datetime = encode({"datetime_value": value})
+        codec_option = CodecOptions(datetime_conversion=DatetimeConversion.DATETIME_CLAMP)
+        decoded_datetime = decode(encoded_datetime, codec_options=codec_option)
+        return safe_transform_datetime(decoded_datetime["datetime_value"], path)
 
     return value
 
 def row_to_singer_record(stream, row, version, time_extracted):
     # pylint: disable=unidiomatic-typecheck
     try:
         row_to_persist = {k:transform_value(v, [k]) for k, v in row.items()
```

### Comparing `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/full_table.py` & `tap-mongodb-3.0.0/tap_mongodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/incremental.py` & `tap-mongodb-3.0.0/tap_mongodb/sync_strategies/incremental.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tap_mongodb/sync_strategies/oplog.py` & `tap-mongodb-3.0.0/tap_mongodb/sync_strategies/oplog.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tap_mongodb.egg-info/SOURCES.txt` & `tap-mongodb-3.0.0/tap_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_cname_restrictions.py` & `tap-mongodb-3.0.0/tests/test_mongodb_cname_restrictions.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_configurable_properties.py` & `tap-mongodb-3.0.0/tests/test_mongodb_configurable_properties.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_datatype.py` & `tap-mongodb-3.0.0/tests/test_mongodb_datatype.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,37 @@
 import re
 import subprocess
 import unittest
 import uuid
 
 from mongodb_common import drop_all_collections, get_test_connection, ensure_environment_variables_set
 from tap_tester import connections, menagerie, runner
+from tap_tester.logger import LOGGER
 
 
 RECORD_COUNT = {}
 
 
-def run_mongodb_javascript(database, js):
+def run_mongodb_javascript(database, js, mongo_version):
     """
     Runs arbitrary javascript against the test Mongo instance. This is
     useful for setting up situations that Python can't handle (e.g.,
     datetime with year 0) for testing.
     """
-    print("Running '{}' against database '{}'".format(js, database))
-    cmd = ["mongo", "-u", os.getenv('TAP_MONGODB_USER'), "-p", os.getenv('TAP_MONGODB_PASSWORD'), "--authenticationDatabase", os.getenv('TAP_MONGODB_DBNAME'), database, "--eval", "eval('{}')".format(js)]
+    LOGGER.info("Running '{}' against database '{}'".format(js, database))
+
+    mongo_shell = "mongosh" if int(mongo_version.split(".")[0]) > 5 else "mongo"
+    cmd = [mongo_shell, "-u", os.getenv('TAP_MONGODB_USER'), "-p", os.getenv('TAP_MONGODB_PASSWORD'), "--authenticationDatabase", os.getenv('TAP_MONGODB_DBNAME'), database, "--eval", "eval('{}')".format(js)]
     subprocess.run(cmd)
 
 
 class MongoDBDatatype(unittest.TestCase):
+    # To compare large dictionaries
+    maxDiff = None
+
     def setUp(self):
         ensure_environment_variables_set()
 
         with get_test_connection() as client:
             ############# Drop all dbs/collections #############
             drop_all_collections(client)
 
@@ -67,15 +73,18 @@
                 "uuid_field": uuid.UUID('3e139ff5-d622-45c6-bf9e-1dfec72820c4'),
                 "dbref_field": bson.dbref.DBRef("some_collection", bson.objectid.ObjectId(b'123456789123'), database='some_database')
             }
 
             client["datatype_db"]["datatype_coll_1"].insert_one(datatype_doc)
 
             # NB: Insert an invalid datetime to confirm that works correctly
-            run_mongodb_javascript("datatype_db", "db.invalid_datatype_coll.insert({ \"date_field\": new ISODate(\"0000-01-01T00:00:00.000Z\") });")
+            mongodb_version = client.server_info()["version"]
+            run_mongodb_javascript(database="datatype_db",
+                                   js="db.invalid_datatype_coll.insert({ \"date_field\": new ISODate(\"0000-01-01T00:00:00.000Z\") });",
+                                   mongo_version=mongodb_version)
 
     def expected_check_streams(self):
         return {
             'datatype_db-datatype_coll_1',
             'datatype_db-invalid_datatype_coll'
         }
 
@@ -228,8 +237,12 @@
             "decimal_field": decimal.Decimal('1.34'),
             'uuid_field': "3e139ff5-d622-45c6-bf9e-1dfec72820c4",
             "dbref_field": {"id": "313233343536373839313233",
                             "database": "some_database",
                             "collection": "some_collection"}
         }
 
-        self.assertEquals(expected_record, records_by_stream['datatype_coll_1']['messages'][1]['data'])
+        dict_keys = list(expected_record.keys())
+        dict_keys.sort()
+
+        self.assertEquals({i: expected_record[i] for i in dict_keys},
+                          {i: records_by_stream['datatype_coll_1']['messages'][1]['data'][i] for i in dict_keys})
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_discovery.py` & `tap-mongodb-3.0.0/tests/test_mongodb_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_fname_restrictions.py` & `tap-mongodb-3.0.0/tests/test_mongodb_fname_restrictions.py`

 * *Files 7% similar despite different names*

```diff
@@ -184,52 +184,52 @@
             object_id = client['simple_db']['simple_coll_2'].find()[1]['_id']
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_2"].delete_one({'_id': object_id})
 
             # Update two documents for each collection
 
             # curor objects do not support negative indicies so set indicies for last two records
-            num_records = client['simple_db']['simple_coll_1'].find().count()
+            num_records = len(list(client['simple_db']['simple_coll_1'].find()))
             last_index = num_records - 1
             sec_last_index = num_records -2
 
             # Not supported in mongodb 4.2 TDL-20088
             # object_id = client['simple_db']['simple_coll_1'].find()[sec_last_index]['_id'] # int.field 48
             # changed_ids.add(object_id)
             # client["simple_db"]["simple_coll_1"].update_one({'_id': object_id},{'$set': {'int.field': -1}})
 
             object_id = client['simple_db']['simple_coll_1'].find()[last_index]['_id'] # int.field 49
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_1"].update_one({'_id': object_id},{'$set': {'string$field': "Updated_1"}})
 
-            num_records = client['simple_db']['simple_coll_2'].find().count()
+            num_records = len(list(client['simple_db']['simple_coll_2'].find()))
             last_index = num_records - 1
             sec_last_index = num_records - 2
 
             # Not supported in mongodb 4.2 TDL-20088
             # object_id = client['simple_db']['simple_coll_2'].find()[sec_last_index]['_id'] # int.field 98
             # changed_ids.add(object_id)
             # client["simple_db"]["simple_coll_2"].update_one({'_id': object_id},{'$set': {'int.field': -1}})
 
             object_id = client['simple_db']['simple_coll_2'].find()[last_index]['_id'] # int.field 99
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_2"].update_one({'_id': object_id},{'$set': {'string$field': "Updated_2"}})
 
             # Insert two documents for each collection
-            last_index = client['simple_db']['simple_coll_1'].find().count()
+            last_index = len(list(client['simple_db']['simple_coll_1'].find()))
             client["simple_db"]["simple_coll_1"].insert_one({"int.field": 50, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_1"].find()[last_index]['_id']
             changed_ids.add(object_id)
 
             last_index += 1 # inserting a new item
             client["simple_db"]["simple_coll_1"].insert_one({"int.field": 51, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_1"].find()[last_index]['_id']
             changed_ids.add(object_id)
 
-            last_index = client['simple_db']['simple_coll_2'].find().count()
+            last_index = len(list(client['simple_db']['simple_coll_2'].find()))
             client["simple_db"]["simple_coll_2"].insert_one({"int.field": 100, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_2"].find()[last_index]['_id']
             changed_ids.add(object_id)
 
             last_index += 1
             client["simple_db"]["simple_coll_2"].insert_one({"int.field": 101, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_2"].find()[last_index]['_id']
@@ -268,24 +268,25 @@
         self.assertEqual(2, len([x['data'] for x in records_by_stream['simple_coll_2'] if x['data'].get('_sdc_deleted_at')]))
         # Verify that the _id of the records sent are the same set as the
         # _ids of the documents changed
         actual = set([ObjectId(x['data']['_id']) for x in records_by_stream['simple_coll_1']]).union(
             set([ObjectId(x['data']['_id']) for x in records_by_stream['simple_coll_2']]))
         self.assertEqual(changed_ids, actual)
 
-        # Verify the updated record values in the db match the tap output file
-        found_id_db = client['simple_db']['simple_coll_1'].find({'string$field': "Updated_1"})[0]['_id']
-        found_id_tap = [ x['data']['_id'] for x in records_by_stream['simple_coll_1']
-                                 if x['data'].get('string$field') == 'Updated_1' ]
-        self.assertEqual(str(found_id_db), found_id_tap[0])
-
-        found_id_db = client['simple_db']['simple_coll_2'].find({'string$field': "Updated_2"})[0]['_id']
-        found_id_tap = [ x['data']['_id'] for x in records_by_stream['simple_coll_2']
-                                 if x['data'].get('string$field') == 'Updated_2' ]
-        self.assertEqual(str(found_id_db), found_id_tap[0])
-
-        # Not supported in mongodb 4.2 TDL-20088. Verify updated record values in db match tap output file
-        # found_int = -1 # one document in each colleciton was updated to have an int value of -1
-        # found_ints_1 = [x['data']['int.field'] for x in records_by_stream['simple_coll_1'] if x['data'].get('int.field')]
-        # found_ints_2 = [x['data']['int.field'] for x in records_by_stream['simple_coll_2'] if x['data'].get('int.field')]
-        # self.assertIn(found_int, found_ints_1)
-        # self.assertIn(found_int, found_ints_2)
+        with get_test_connection() as client:
+            # Verify the updated record values in the db match the tap output file
+            found_id_db = client['simple_db']['simple_coll_1'].find({'string$field': "Updated_1"})[0]['_id']
+            found_id_tap = [ x['data']['_id'] for x in records_by_stream['simple_coll_1']
+                                    if x['data'].get('string$field') == 'Updated_1' ]
+            self.assertEqual(str(found_id_db), found_id_tap[0])
+
+            found_id_db = client['simple_db']['simple_coll_2'].find({'string$field': "Updated_2"})[0]['_id']
+            found_id_tap = [ x['data']['_id'] for x in records_by_stream['simple_coll_2']
+                                    if x['data'].get('string$field') == 'Updated_2' ]
+            self.assertEqual(str(found_id_db), found_id_tap[0])
+
+            # Not supported in mongodb 4.2 TDL-20088. Verify updated record values in db match tap output file
+            # found_int = -1 # one document in each colleciton was updated to have an int value of -1
+            # found_ints_1 = [x['data']['int.field'] for x in records_by_stream['simple_coll_1'] if x['data'].get('int.field')]
+            # found_ints_2 = [x['data']['int.field'] for x in records_by_stream['simple_coll_2'] if x['data'].get('int.field')]
+            # self.assertIn(found_int, found_ints_1)
+            # self.assertIn(found_int, found_ints_2)
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_full_table.py` & `tap-mongodb-3.0.0/tests/test_mongodb_full_table.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_full_table_id.py` & `tap-mongodb-3.0.0/tests/test_mongodb_full_table_id.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_full_table_interruptible.py` & `tap-mongodb-3.0.0/tests/test_mongodb_full_table_interruptible.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_id_pk_variations.py` & `tap-mongodb-3.0.0/tests/test_mongodb_id_pk_variations.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_incremental.py` & `tap-mongodb-3.0.0/tests/test_mongodb_incremental.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from unittest import TestCase
 
 from mongodb_common import drop_all_collections, get_test_connection, ensure_environment_variables_set
 from tap_tester import connections, menagerie, runner
 
 
 RECORD_COUNT = {}
-VALID_REPLICATION_TYPES = {'datetime', 'Int64', 'float', 'int', 'str', 'Timestamp', 'UUID'}
+VALID_REPLICATION_TYPES = {'datetime', 'Int64', 'float', 'int', 'str', 'Timestamp', 'UUID', 'Binary'}
 
 def z_string_generator(size=6):
     return 'z' * size
 
 def generate_simple_coll_docs(num_docs):
     docs = []
     start_datetime = datetime(2018, 1, 1, 19, 29, 14, 578000)
@@ -406,17 +406,18 @@
                 actual = set([x['data']['int_field'] for x in records_by_stream[stream_name]])
                 self.assertEqual(self.expected_incremental_int_fields()[stream_name], actual)
 
         ##############################################################################
         # Verify that data is not replicated when non replication key is updated
         ##############################################################################
 
-        # Sampling a document from a collection which we know it exists because of the data set up
-        no_rep_doc_coll_1 = client["simple_db"]["simple_coll_1"].find_one({"int_field": 20})
-        client["simple_db"]["simple_coll_1"].find_one_and_update({"_id": no_rep_doc_coll_1["_id"]}, {"$set": {"string_field": 'No_replication'}})
+        with get_test_connection() as client:
+            # Sampling a document from a collection which we know it exists because of the data set up
+            no_rep_doc_coll_1 = client["simple_db"]["simple_coll_1"].find_one({"int_field": 20})
+            client["simple_db"]["simple_coll_1"].find_one_and_update({"_id": no_rep_doc_coll_1["_id"]}, {"$set": {"string_field": 'No_replication'}})
 
         # Run sync
         sync_job_name = runner.run_sync_mode(self, conn_id)
         exit_status = menagerie.get_exit_status(conn_id, sync_job_name)
         menagerie.verify_sync_exit_status(self, exit_status, sync_job_name)
         record_count_by_stream = runner.examine_target_output_file(self,
                                                                    conn_id,
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_incremental_open_transactions.py` & `tap-mongodb-3.0.0/tests/test_mongodb_oplog.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import random
 import string
 import unittest
+from bson import ObjectId
 
 from mongodb_common import drop_all_collections, get_test_connection, ensure_environment_variables_set
 from tap_tester import connections, menagerie, runner
 
 
 RECORD_COUNT = {}
 
@@ -15,294 +16,232 @@
 
 def generate_simple_coll_docs(num_docs):
     docs = []
     for int_value in range(num_docs):
         docs.append({"int_field": int_value, "string_field": random_string_generator()})
     return docs
 
-class MongoDBOpenTransactions(unittest.TestCase):
+class MongoDBOplog(unittest.TestCase):
+    def setUp(self):
 
-    def expected_check_streams_sync_1(self):
-        return {
-            'simple_db-simple_coll_1',
-            'simple_db-simple_coll_2',
-            'simple_db-simple_coll_3'
-        }
+        ensure_environment_variables_set()
 
-    def expected_check_streams_sync_2(self):
-        return {
-            'simple_db-simple_coll_1',
-            'simple_db-simple_coll_2',
-            'simple_db-simple_coll_3'
-        }
+        with get_test_connection() as client:
+            ############# Drop all dbs/collections #############
+            drop_all_collections(client)
 
-    def expected_pks_1(self):
-        return {
-            'simple_db_simple_coll_1': {'_id'},
-            'simple_db_simple_coll_2': {'_id'},
-            'simple_db_simple_coll_3': {'_id'}
-        }
+            ############# Add simple collections #############
+            # simple_coll_1 has 50 documents
+            client["simple_db"]["simple_coll_1"].insert_many(generate_simple_coll_docs(50))
 
-    def expected_pks_2(self):
-        return {
-            'simple_db_simple_coll_1': {'_id'},
-            'simple_db_simple_coll_2': {'_id'},
-            'simple_db_simple_coll_3': {'_id'}
-        }
+            # simple_coll_2 has 100 documents
+            client["simple_db"]["simple_coll_2"].insert_many(generate_simple_coll_docs(100))
 
-    def expected_row_counts_sync_1(self):
-        return {
-            'simple_db_simple_coll_1': 10,
-            'simple_db_simple_coll_2': 20,
-            'simple_db_simple_coll_3': 0
-        }
 
-    def expected_row_counts_sync_2(self):
-        return {
-            'simple_db_simple_coll_1': 2,
-            'simple_db_simple_coll_2': 2,
-            'simple_db_simple_coll_3': 5
-        }
 
-    def expected_row_counts_sync_3(self):
-        return {
-            'simple_db_simple_coll_1': 0,
-            'simple_db_simple_coll_2': 0,
-            'simple_db_simple_coll_3': 0
-        }
 
-    def expected_sync_streams_1(self):
+    def expected_check_streams(self):
         return {
-            'simple_db_simple_coll_1',
-            'simple_db_simple_coll_2',
-            'simple_db_simple_coll_3'
+            'simple_db-simple_coll_1',
+            'simple_db-simple_coll_2',
         }
 
-    def expected_sync_streams_2(self):
+    def expected_pks(self):
         return {
-            'simple_db_simple_coll_1',
-            'simple_db_simple_coll_2',
-            'simple_db_simple_coll_3'
+            'simple_coll_1': {'_id'},
+            'simple_coll_2': {'_id'},
         }
 
-    def expected_pk_values_2(self):
+    def expected_row_counts(self):
         return {
-            'simple_db_simple_coll_1': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
-            'simple_db_simple_coll_2': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
-            'simple_db_simple_coll_3': [] # insert to coll 3 is not committed in session 2, hence we are expecting no records to be replicated
+            'simple_coll_1': 50,
+            'simple_coll_2': 100,
         }
 
-    def expected_pk_values_3(self):
+
+    def expected_sync_streams(self):
         return {
-            'simple_db_simple_coll_1': [9, 11], # bookmarked value = 9 and updated value in test = 11
-            'simple_db_simple_coll_2': [19, 21], # bookmarked value = 19 and updated value in test = 21
-            'simple_db_simple_coll_3': [0, 1, 2, 3, 4]
+            'simple_coll_1',
+            'simple_coll_2'
         }
 
     def name(self):
-        return "tap_tester_mongodb_open_transaction"
+        return "tap_tester_mongodb_oplog"
 
     def tap_name(self):
         return "tap-mongodb"
 
     def get_type(self):
         return "platform.mongodb"
 
     def get_credentials(self):
         return {'password': os.getenv('TAP_MONGODB_PASSWORD')}
 
     def get_properties(self):
         return {'host' : os.getenv('TAP_MONGODB_HOST'),
                 'port' : os.getenv('TAP_MONGODB_PORT'),
                 'user' : os.getenv('TAP_MONGODB_USER'),
-                'database' : os.getenv('TAP_MONGODB_DBNAME'),
-                'include_schemas_in_destination_stream_name': 'true'
+                'database' : os.getenv('TAP_MONGODB_DBNAME')
         }
 
+
     def test_run(self):
 
-        ensure_environment_variables_set()
+        conn_id = connections.ensure_connection(self)
+
+        #  -------------------------------
+        # -----------  Discovery ----------
+        #  -------------------------------
+
+        # run in discovery mode
+        check_job_name = runner.run_check_mode(self, conn_id)
+
+        # verify check  exit codes
+        exit_status = menagerie.get_exit_status(conn_id, check_job_name)
+        menagerie.verify_check_exit_status(self, exit_status, check_job_name)
+
+        # verify the tap discovered the right streams
+        found_catalogs = menagerie.get_catalogs(conn_id)
+
+        # assert we find the correct streams
+        self.assertEqual(self.expected_check_streams(),
+                         {c['tap_stream_id'] for c in found_catalogs})
+
+
 
+        for tap_stream_id in self.expected_check_streams():
+            found_stream = [c for c in found_catalogs if c['tap_stream_id'] == tap_stream_id][0]
+
+            # assert that the pks are correct
+            self.assertEqual(self.expected_pks()[found_stream['stream_name']],
+                             set(found_stream.get('metadata', {}).get('table-key-properties')))
+
+            # assert that the row counts are correct
+            self.assertEqual(self.expected_row_counts()[found_stream['stream_name']],
+                             found_stream.get('metadata', {}).get('row-count'))
+
+        #  -----------------------------------
+        # ----------- Initial Full Table ---------
+        #  -----------------------------------
+        # Select simple_coll_1 and simple_coll_2 streams and add replication method metadata
+        for stream_catalog in found_catalogs:
+            annotated_schema = menagerie.get_annotated_schema(conn_id, stream_catalog['stream_id'])
+            additional_md = [{ "breadcrumb" : [], "metadata" : {'replication-method' : 'LOG_BASED'}}]
+            selected_metadata = connections.select_catalog_and_fields_via_metadata(conn_id,
+                                                                                    stream_catalog,
+                                                                                    annotated_schema,
+                                                                                    additional_md)
+
+        # Run sync
+        sync_job_name = runner.run_sync_mode(self, conn_id)
+
+        exit_status = menagerie.get_exit_status(conn_id, sync_job_name)
+        menagerie.verify_sync_exit_status(self, exit_status, sync_job_name)
+
+
+        # verify the persisted schema was correct
+        records_by_stream = runner.get_records_from_target_output()
+
+        # assert that each of the streams that we synced are the ones that we expect to see
+        record_count_by_stream = runner.examine_target_output_file(self,
+                                                                   conn_id,
+                                                                   self.expected_sync_streams(),
+                                                                   self.expected_pks())
+
+        # Verify that the full table was synced
+        for tap_stream_id in self.expected_sync_streams():
+            self.assertGreaterEqual(record_count_by_stream[tap_stream_id],self.expected_row_counts()[tap_stream_id])
+
+        # Verify that we have 'initial_full_table_complete' bookmark
+        state = menagerie.get_state(conn_id)
+        first_versions = {}
+
+        for tap_stream_id in self.expected_check_streams():
+            # assert that the state has an initial_full_table_complete == True
+            self.assertTrue(state['bookmarks'][tap_stream_id]['initial_full_table_complete'])
+            # assert that there is a version bookmark in state
+            first_versions[tap_stream_id] = state['bookmarks'][tap_stream_id]['version']
+            self.assertIsNotNone(first_versions[tap_stream_id])
+            # Verify that we have a oplog_ts_time and oplog_ts_inc bookmark
+            self.assertIsNotNone(state['bookmarks'][tap_stream_id]['oplog_ts_time'])
+            self.assertIsNotNone(state['bookmarks'][tap_stream_id]['oplog_ts_inc'])
+
+
+        changed_ids = set()
         with get_test_connection() as client:
-            # drop all dbs/collections
-            drop_all_collections(client)
+            # Delete two documents for each collection
+
+            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 0})[0]['_id'])
+            client["simple_db"]["simple_coll_1"].delete_one({'int_field': 0})
+
+            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 1})[0]['_id'])
+            client["simple_db"]["simple_coll_1"].delete_one({'int_field': 1})
+
+            changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 0})[0]['_id'])
+            client["simple_db"]["simple_coll_2"].delete_one({'int_field': 0})
+
+            changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 1})[0]['_id'])
+            client["simple_db"]["simple_coll_2"].delete_one({'int_field': 1})
+
+            # Update two documents for each collection
+            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 48})[0]['_id'])
+            client["simple_db"]["simple_coll_1"].update_one({'int_field': 48},{'$set': {'int_field': -1}})
+
+            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 49})[0]['_id'])
+            client["simple_db"]["simple_coll_1"].update_one({'int_field': 49},{'$set': {'int_field': -1}})
+
+            changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 98})[0]['_id'])
+            client["simple_db"]["simple_coll_2"].update_one({'int_field': 98},{'$set': {'int_field': -1}})
+
+            changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 99})[0]['_id'])
+            client["simple_db"]["simple_coll_2"].update_one({'int_field': 99},{'$set': {'int_field': -1}})
+
+            # Insert two documents for each collection
+            client["simple_db"]["simple_coll_1"].insert_one({"int_field": 50, "string_field": random_string_generator()})
+            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 50})[0]['_id'])
+
+            client["simple_db"]["simple_coll_1"].insert_one({"int_field": 51, "string_field": random_string_generator()})
+            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 51})[0]['_id'])
+
+            client["simple_db"]["simple_coll_2"].insert_one({"int_field": 100, "string_field": random_string_generator()})
+            changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 100})[0]['_id'])
+
+            client["simple_db"]["simple_coll_2"].insert_one({"int_field": 101, "string_field": random_string_generator()})
+            changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 101})[0]['_id'])
+
+        #  -----------------------------------
+        # ----------- Subsequent Oplog Sync ---------
+        #  -----------------------------------
+
+        # Run sync
+
+        sync_job_name = runner.run_sync_mode(self, conn_id)
+
+        exit_status = menagerie.get_exit_status(conn_id, sync_job_name)
+        menagerie.verify_sync_exit_status(self, exit_status, sync_job_name)
+
+
+        # verify the persisted schema was correct
+        messages_by_stream = runner.get_records_from_target_output()
+        records_by_stream = {}
+        for stream_name in self.expected_sync_streams():
+            records_by_stream[stream_name] = [x for x in messages_by_stream[stream_name]['messages'] if x.get('action') == 'upsert']
 
-            # Create session 1 and insert docs to simple_coll_1 & simple_coll_2
 
-            #################
-            # Session 1
-            #################
-
-            session1 = client.start_session()
-
-            session1.start_transaction()
-
-            # simple_coll_1 has 10 documents
-            client["simple_db"]["simple_coll_1"].insert_many(generate_simple_coll_docs(10))
-
-            # simple_coll_2 has 20 documents
-            client["simple_db"]["simple_coll_2"].insert_many(generate_simple_coll_docs(20))
-
-            session1.commit_transaction()
-
-            # Create session 2
-            '''
-                create empty collection
-                update documents in simple_coll_1 & simple_coll_2 and tie to session 2
-                insert documents in simple_coll_3 and tie to session 2
-                execute the sync with uncommitted changes
-                validate that the uncommitted changes are not replicated by the sync
-            '''
-            ################
-            # Session 2
-            ################
-
-            session2 = client.start_session()
-
-            session2.start_transaction()
-
-            # simple_coll_3 is an empty collection
-            client["simple_db"].create_collection("simple_coll_3")
-
-            # update document from coll 1 and coll 2
-            client["simple_db"]["simple_coll_1"].update_one({"int_field": 5}, {"$set": {"int_field": 11}}, session=session2)
-            client["simple_db"]["simple_coll_2"].update_one({"int_field": 10}, {"$set": {"int_field": 21}}, session=session2)
-
-            # insert document to coll 3
-            client["simple_db"]["simple_coll_3"].insert_many(generate_simple_coll_docs(5), session=session2)
-
-            # deletes do not matter in incremental replication, invalid scenario to test
-
-            conn_id = connections.ensure_connection(self)
-
-            # run in discovery mode
-            check_job_name = runner.run_check_mode(self, conn_id)
-
-            # verify check exit codes
-            exit_status = menagerie.get_exit_status(conn_id, check_job_name)
-            menagerie.verify_check_exit_status(self, exit_status, check_job_name)
-
-            # verify the tap discovered the right streams
-            found_catalogs = menagerie.get_catalogs(conn_id)
-
-            # assert we find the correct streams which includes all collections which are part of session1 and session2
-            self.assertEqual(self.expected_check_streams_sync_1(),
-                             {c['tap_stream_id'] for c in found_catalogs})
-
-            # Select streams and add replication method metadata
-            for stream_catalog in found_catalogs:
-                annotated_schema = menagerie.get_annotated_schema(conn_id, stream_catalog['stream_id'])
-                additional_md = [{ "breadcrumb" : [], "metadata" : {'replication-method' : 'INCREMENTAL', 'replication_key': 'int_field'}}]
-                selected_metadata = connections.select_catalog_and_fields_via_metadata(conn_id,
-                                                                                        stream_catalog,
-                                                                                        annotated_schema,
-                                                                                        additional_md)
-
-            # run full table sync
-            sync_1 = runner.run_sync_mode(self, conn_id)
-
-            # check exit status
-            exit_status = menagerie.get_exit_status(conn_id, sync_1)
-            menagerie.verify_sync_exit_status(self, exit_status, sync_1)
-
-            # streams that we synced are the ones that we expect to see
-            records_by_stream = runner.get_records_from_target_output()
-            record_count_by_stream = runner.examine_target_output_file(self,
-                                                                       conn_id,
-                                                                       self.expected_sync_streams_1(),
-                                                                       self.expected_pks_1())
-
-            # validate the record count in collections which are part of session1 and session2, should not read updates on coll 1 and coll 2 and insert on coll 3. Because the transaction is not committed
-            self.assertEqual(self.expected_row_counts_sync_1(), record_count_by_stream)
-
-            # validate there are no duplicates replicated as part of sync1
-            records_2 = {}
-            pk_dict_2 = {}
-            for stream in self.expected_sync_streams_1():
-                records_2[stream] = [x for x in records_by_stream[stream]['messages'] if x.get('action') == 'upsert']
-                pk_2 = []
-                for record in range(len(records_2[stream])):
-                    pk_2.append(records_2[stream][record]['data']['int_field'])
-                pk_dict_2[stream] = pk_2
-
-            self.assertEqual(self.expected_pk_values_2(), pk_dict_2)
-
-            session2.commit_transaction()
-
-            # Create session 3
-            '''
-               Execute another sync
-               Validate that the documents committed as part of session 2 should now be replicated in sync_2
-            '''
-            ################
-            # Session 3
-            ################
-
-            session3 = client.start_session()
-
-            session3.start_transaction()
-
-            # Run 2nd sync
-            # run in discovery mode
-
-            sync_2 = runner.run_sync_mode(self, conn_id)
-            exit_status_2 = menagerie.get_exit_status(conn_id, sync_2)
-            menagerie.verify_sync_exit_status(self, exit_status_2, sync_2)
-
-            records_by_stream_2 = runner.get_records_from_target_output()
-            record_count_by_stream_2 = runner.examine_target_output_file(self,
-                                                                         conn_id,
-                                                                         self.expected_sync_streams_2(),
-                                                                         self.expected_pks_2())
-            # validate that we see the updates to coll 1 and coll 2 and insert to coll 3 in the 2nd sync
-            # we see 2 records for coll 1 and coll 2, 1 record for update and the other record for the bookmarked record
-            self.assertEqual(self.expected_row_counts_sync_2(), record_count_by_stream_2)
-
-            # validate there are no duplicates replicated as part of sync1
-            records_3 = {}
-            pk_dict_3 = {}
-            for stream in self.expected_sync_streams_1():
-                records_3[stream] = [x for x in records_by_stream_2[stream]['messages'] if x.get('action') == 'upsert']
-                pk_3 = []
-                for record in range(len(records_3[stream])):
-                    pk_3.append(records_3[stream][record]['data']['int_field'])
-                pk_dict_3[stream] = pk_3
-
-            self.assertEqual(self.expected_pk_values_3(), pk_dict_3)
-
-
-            # Test case to validate tap behaviour when we delete bookmarked document and run sync
-            state_2 = menagerie.get_state(conn_id)
-
-            for stream in self.expected_check_streams_sync_1():
-                rep_key_value = state_2['bookmarks'][stream]['replication_key_value']
-                if stream == 'simple_db-simple_coll_1':
-                    collection = 'simple_coll_1'
-                elif stream == 'simple_db-simple_coll_2':
-                    collection = 'simple_coll_2'
-                elif stream == 'simple_db-simple_coll_3':
-                    collection = 'simple_coll_3'
-                client["simple_db"][collection].delete_one({"int_field": int(rep_key_value)}, session=session3)
-
-            session3.commit_transaction()
-
-            '''
-               Execute the sync, after the commit on session 3
-               Session 3 commits includes deleting the bookmarked value in each of the collection
-               Validate the state does not change after deleting the bookmarked value
-               Validate that the sync does not replicate any documents
-            '''
-            state_3 = menagerie.get_state(conn_id)
-            sync_3 = runner.run_sync_mode(self, conn_id)
-            exit_status_3 = menagerie.get_exit_status(conn_id, sync_3)
-            menagerie.verify_sync_exit_status(self, exit_status_3, sync_3)
-            records_by_stream_3 = runner.get_records_from_target_output()
-            record_count_by_stream_3 = runner.examine_target_output_file(self,
-                                                                         conn_id,
-                                                                         self.expected_sync_streams_2(),
-                                                                         self.expected_pks_2())
+        # assert that each of the streams that we synced are the ones that we expect to see
+        record_count_by_stream = runner.examine_target_output_file(self,
+                                                                   conn_id,
+                                                                   self.expected_sync_streams(),
+                                                                   self.expected_pks())
 
-            # validate that we see 0 records being replicated because we deleted the bookmark value on each of the collection
-            self.assertEqual(self.expected_row_counts_sync_3(), record_count_by_stream_3)
+        # Verify that we got at least 6 records due to changes
+        # (could be more due to overlap in gte oplog clause)
+        for k,v in record_count_by_stream.items():
+            self.assertGreaterEqual(v, 6)
 
-            # validate that the state value has not changed after deleting the bookmarked value in each collection
-            self.assertEqual(state_2, state_3)
+        # Verify that we got 2 records with _SDC_DELETED_AT
+        self.assertEqual(2, len([x['data'] for x in records_by_stream['simple_coll_1'] if x['data'].get('_sdc_deleted_at')]))
+        self.assertEqual(2, len([x['data'] for x in records_by_stream['simple_coll_2'] if x['data'].get('_sdc_deleted_at')]))
+        # Verify that the _id of the records sent are the same set as the
+        # _ids of the documents changed
+        actual = set([ObjectId(x['data']['_id']) for x in records_by_stream['simple_coll_1']]).union(set([ObjectId(x['data']['_id']) for x in records_by_stream['simple_coll_2']]))
+        self.assertEqual(changed_ids, actual)
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_index.py` & `tap-mongodb-3.0.0/tests/test_mongodb_index.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_log_based_interruptible.py` & `tap-mongodb-3.0.0/tests/test_mongodb_log_based_interruptible.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_name_restrictions.py` & `tap-mongodb-3.0.0/tests/test_mongodb_name_restrictions.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,50 +186,50 @@
             object_id = client['simple_db']['simple_coll_2'].find()[1]['_id']
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_2"].delete_one({'_id': object_id})
 
             # Update two documents for each collection
 
             # curor objects do not support negative indicies so set indicies for last two records
-            num_records = client['simple_db']['simple_coll_1'].find().count()
+            num_records = len(list(client['simple_db']['simple_coll_1'].find()))
             last_index = num_records - 1
             sec_last_index = num_records -2
 
             object_id = client['simple_db']['simple_coll_1'].find()[sec_last_index]['_id'] # int.field 48
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_1"].update_one({'_id': object_id},{'$set': {'int.field': -1}})
 
             object_id = client['simple_db']['simple_coll_1'].find()[last_index]['_id'] # int.field 49
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_1"].update_one({'_id': object_id},{'$set': {'int.field': -1}})
 
-            num_records = client['simple_db']['simple_coll_2'].find().count()
+            num_records = len(list(client['simple_db']['simple_coll_2'].find()))
             last_index = num_records - 1
             sec_last_index = num_records - 2
 
             object_id = client['simple_db']['simple_coll_2'].find()[sec_last_index]['_id'] # int.field 98
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_2"].update_one({'_id': object_id},{'$set': {'int.field': -1}})
 
             object_id = client['simple_db']['simple_coll_2'].find()[last_index]['_id'] # int.field 99
             changed_ids.add(object_id)
             client["simple_db"]["simple_coll_2"].update_one({'_id': object_id},{'$set': {'int.field': -1}})
 
             # Insert two documents for each collection
-            last_index = client['simple_db']['simple_coll_1'].find().count()
+            last_index = len(list(client['simple_db']['simple_coll_1'].find()))
             client["simple_db"]["simple_coll_1"].insert_one({"int.field": 50, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_1"].find()[last_index]['_id']
             changed_ids.add(object_id)
 
             last_index += 1 # inserting a new item
             client["simple_db"]["simple_coll_1"].insert_one({"int.field": 51, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_1"].find()[last_index]['_id']
             changed_ids.add(object_id)
 
-            last_index = client['simple_db']['simple_coll_2'].find().count()
+            last_index = len(list(client['simple_db']['simple_coll_2'].find()))
             client["simple_db"]["simple_coll_2"].insert_one({"int.field": 100, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_2"].find()[last_index]['_id']
             changed_ids.add(object_id)
 
             last_index += 1
             client["simple_db"]["simple_coll_2"].insert_one({"int.field": 101, "string$field": random_string_generator()})
             object_id = client["simple_db"]["simple_coll_2"].find()[last_index]['_id']
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_namespace_restrictions.py` & `tap-mongodb-3.0.0/tests/test_mongodb_namespace_restrictions.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_oplog.py` & `tap-mongodb-3.0.0/tests/test_mongodb_oplog_bookmarks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
+import pymongo
 import random
 import string
+import time
 import unittest
-from bson import ObjectId
 
 from mongodb_common import drop_all_collections, get_test_connection, ensure_environment_variables_set
 from tap_tester import connections, menagerie, runner
 
 
 RECORD_COUNT = {}
 
@@ -16,33 +17,29 @@
 
 def generate_simple_coll_docs(num_docs):
     docs = []
     for int_value in range(num_docs):
         docs.append({"int_field": int_value, "string_field": random_string_generator()})
     return docs
 
-class MongoDBOplog(unittest.TestCase):
+class MongoDBOplogBookmarks(unittest.TestCase):
     def setUp(self):
 
         ensure_environment_variables_set()
 
         with get_test_connection() as client:
-            ############# Drop all dbs/collections #############
             drop_all_collections(client)
 
-            ############# Add simple collections #############
             # simple_coll_1 has 50 documents
             client["simple_db"]["simple_coll_1"].insert_many(generate_simple_coll_docs(50))
 
             # simple_coll_2 has 100 documents
             client["simple_db"]["simple_coll_2"].insert_many(generate_simple_coll_docs(100))
 
 
-
-
     def expected_check_streams(self):
         return {
             'simple_db-simple_coll_1',
             'simple_db-simple_coll_2',
         }
 
     def expected_pks(self):
@@ -51,40 +48,42 @@
             'simple_coll_2': {'_id'},
         }
 
     def expected_row_counts(self):
         return {
             'simple_coll_1': 50,
             'simple_coll_2': 100,
+
         }
 
 
     def expected_sync_streams(self):
         return {
             'simple_coll_1',
-            'simple_coll_2'
+            'simple_coll_2',
         }
 
     def name(self):
-        return "tap_tester_mongodb_oplog"
+        return "tap_tester_mongodb_oplog_bookmarks"
 
     def tap_name(self):
         return "tap-mongodb"
 
     def get_type(self):
         return "platform.mongodb"
 
     def get_credentials(self):
         return {'password': os.getenv('TAP_MONGODB_PASSWORD')}
 
     def get_properties(self):
-        return {'host' : os.getenv('TAP_MONGODB_HOST'),
-                'port' : os.getenv('TAP_MONGODB_PORT'),
-                'user' : os.getenv('TAP_MONGODB_USER'),
-                'database' : os.getenv('TAP_MONGODB_DBNAME')
+        return {
+            'host' : os.getenv('TAP_MONGODB_HOST'),
+            'port' : os.getenv('TAP_MONGODB_PORT'),
+            'user' : os.getenv('TAP_MONGODB_USER'),
+            'database' : os.getenv('TAP_MONGODB_DBNAME')
         }
 
 
     def test_run(self):
 
         conn_id = connections.ensure_connection(self)
 
@@ -102,38 +101,38 @@
         # verify the tap discovered the right streams
         found_catalogs = menagerie.get_catalogs(conn_id)
 
         # assert we find the correct streams
         self.assertEqual(self.expected_check_streams(),
                          {c['tap_stream_id'] for c in found_catalogs})
 
-
-
         for tap_stream_id in self.expected_check_streams():
             found_stream = [c for c in found_catalogs if c['tap_stream_id'] == tap_stream_id][0]
 
             # assert that the pks are correct
             self.assertEqual(self.expected_pks()[found_stream['stream_name']],
                              set(found_stream.get('metadata', {}).get('table-key-properties')))
 
             # assert that the row counts are correct
             self.assertEqual(self.expected_row_counts()[found_stream['stream_name']],
                              found_stream.get('metadata', {}).get('row-count'))
 
         #  -----------------------------------
         # ----------- Initial Full Table ---------
         #  -----------------------------------
-        # Select simple_coll_1 and simple_coll_2 streams and add replication method metadata
+        # Select simple_coll_1 and add replication method metadata
+        additional_md = [{ "breadcrumb" : [],
+                           "metadata" : {'replication-method' : 'LOG_BASED'}}]
         for stream_catalog in found_catalogs:
-            annotated_schema = menagerie.get_annotated_schema(conn_id, stream_catalog['stream_id'])
-            additional_md = [{ "breadcrumb" : [], "metadata" : {'replication-method' : 'LOG_BASED'}}]
-            selected_metadata = connections.select_catalog_and_fields_via_metadata(conn_id,
-                                                                                    stream_catalog,
-                                                                                    annotated_schema,
-                                                                                    additional_md)
+            if stream_catalog['tap_stream_id'] == 'simple_db-simple_coll_1':
+                annotated_schema = menagerie.get_annotated_schema(conn_id, stream_catalog['stream_id'])
+                selected_metadata = connections.select_catalog_and_fields_via_metadata(conn_id,
+                                                                                       stream_catalog,
+                                                                                       annotated_schema,
+                                                                                       additional_md)
 
         # Run sync
         sync_job_name = runner.run_sync_mode(self, conn_id)
 
         exit_status = menagerie.get_exit_status(conn_id, sync_job_name)
         menagerie.verify_sync_exit_status(self, exit_status, sync_job_name)
 
@@ -144,104 +143,91 @@
         # assert that each of the streams that we synced are the ones that we expect to see
         record_count_by_stream = runner.examine_target_output_file(self,
                                                                    conn_id,
                                                                    self.expected_sync_streams(),
                                                                    self.expected_pks())
 
         # Verify that the full table was synced
-        for tap_stream_id in self.expected_sync_streams():
-            self.assertGreaterEqual(record_count_by_stream[tap_stream_id],self.expected_row_counts()[tap_stream_id])
+        tap_stream_id = 'simple_db-simple_coll_1'
+        self.assertGreaterEqual(record_count_by_stream['simple_coll_1'],
+                                self.expected_row_counts()['simple_coll_1'])
 
         # Verify that we have 'initial_full_table_complete' bookmark
         state = menagerie.get_state(conn_id)
         first_versions = {}
 
-        for tap_stream_id in self.expected_check_streams():
-            # assert that the state has an initial_full_table_complete == True
-            self.assertTrue(state['bookmarks'][tap_stream_id]['initial_full_table_complete'])
-            # assert that there is a version bookmark in state
-            first_versions[tap_stream_id] = state['bookmarks'][tap_stream_id]['version']
-            self.assertIsNotNone(first_versions[tap_stream_id])
-            # Verify that we have a oplog_ts_time and oplog_ts_inc bookmark
-            self.assertIsNotNone(state['bookmarks'][tap_stream_id]['oplog_ts_time'])
-            self.assertIsNotNone(state['bookmarks'][tap_stream_id]['oplog_ts_inc'])
+        # assert that the state has an initial_full_table_complete == True
+        self.assertTrue(state['bookmarks'][tap_stream_id]['initial_full_table_complete'])
+        # assert that there is a version bookmark in state
+        first_versions[tap_stream_id] = state['bookmarks'][tap_stream_id]['version']
+        self.assertIsNotNone(first_versions[tap_stream_id])
+        # Verify that we have a oplog_ts_time and oplog_ts_inc bookmark
+        self.assertIsNotNone(state['bookmarks'][tap_stream_id]['oplog_ts_time'])
+        self.assertIsNotNone(state['bookmarks'][tap_stream_id]['oplog_ts_inc'])
 
 
-        changed_ids = set()
-        with get_test_connection() as client:
-            # Delete two documents for each collection
 
-            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 0})[0]['_id'])
-            client["simple_db"]["simple_coll_1"].delete_one({'int_field': 0})
+        # Insert records to coll_1 to get the bookmark to be a ts on coll_1
+        with get_test_connection() as client:
+            client["simple_db"]["simple_coll_1"].insert_one({"int_field": 101, "string_field": random_string_generator()})
+        sync_job_name = runner.run_sync_mode(self, conn_id)
 
-            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 1})[0]['_id'])
-            client["simple_db"]["simple_coll_1"].delete_one({'int_field': 1})
 
+        changed_ids = set()
+        with get_test_connection() as client:
+            # Make changes to not selected collection
             changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 0})[0]['_id'])
             client["simple_db"]["simple_coll_2"].delete_one({'int_field': 0})
 
             changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 1})[0]['_id'])
             client["simple_db"]["simple_coll_2"].delete_one({'int_field': 1})
 
-            # Update two documents for each collection
-            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 48})[0]['_id'])
-            client["simple_db"]["simple_coll_1"].update_one({'int_field': 48},{'$set': {'int_field': -1}})
-
-            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 49})[0]['_id'])
-            client["simple_db"]["simple_coll_1"].update_one({'int_field': 49},{'$set': {'int_field': -1}})
-
             changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 98})[0]['_id'])
             client["simple_db"]["simple_coll_2"].update_one({'int_field': 98},{'$set': {'int_field': -1}})
 
             changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 99})[0]['_id'])
             client["simple_db"]["simple_coll_2"].update_one({'int_field': 99},{'$set': {'int_field': -1}})
 
-            # Insert two documents for each collection
-            client["simple_db"]["simple_coll_1"].insert_one({"int_field": 50, "string_field": random_string_generator()})
-            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 50})[0]['_id'])
-
-            client["simple_db"]["simple_coll_1"].insert_one({"int_field": 51, "string_field": random_string_generator()})
-            changed_ids.add(client['simple_db']['simple_coll_1'].find({'int_field': 51})[0]['_id'])
-
             client["simple_db"]["simple_coll_2"].insert_one({"int_field": 100, "string_field": random_string_generator()})
             changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 100})[0]['_id'])
 
             client["simple_db"]["simple_coll_2"].insert_one({"int_field": 101, "string_field": random_string_generator()})
             changed_ids.add(client['simple_db']['simple_coll_2'].find({'int_field': 101})[0]['_id'])
 
         #  -----------------------------------
         # ----------- Subsequent Oplog Sync ---------
         #  -----------------------------------
 
         # Run sync
-
         sync_job_name = runner.run_sync_mode(self, conn_id)
 
         exit_status = menagerie.get_exit_status(conn_id, sync_job_name)
         menagerie.verify_sync_exit_status(self, exit_status, sync_job_name)
 
-
         # verify the persisted schema was correct
         messages_by_stream = runner.get_records_from_target_output()
-        records_by_stream = {}
-        for stream_name in self.expected_sync_streams():
-            records_by_stream[stream_name] = [x for x in messages_by_stream[stream_name]['messages'] if x.get('action') == 'upsert']
-
+        records_by_stream = {
+            'simple_coll_1': [x
+                              for x in messages_by_stream['simple_coll_1']['messages']
+                              if x.get('action') == 'upsert']
+        }
 
         # assert that each of the streams that we synced are the ones that we expect to see
         record_count_by_stream = runner.examine_target_output_file(self,
                                                                    conn_id,
                                                                    self.expected_sync_streams(),
                                                                    self.expected_pks())
 
-        # Verify that we got at least 6 records due to changes
-        # (could be more due to overlap in gte oplog clause)
-        for k,v in record_count_by_stream.items():
-            self.assertGreaterEqual(v, 6)
-
-        # Verify that we got 2 records with _SDC_DELETED_AT
-        self.assertEqual(2, len([x['data'] for x in records_by_stream['simple_coll_1'] if x['data'].get('_sdc_deleted_at')]))
-        self.assertEqual(2, len([x['data'] for x in records_by_stream['simple_coll_2'] if x['data'].get('_sdc_deleted_at')]))
-        # Verify that the _id of the records sent are the same set as the
-        # _ids of the documents changed
-        actual = set([ObjectId(x['data']['_id']) for x in records_by_stream['simple_coll_1']]).union(set([ObjectId(x['data']['_id']) for x in records_by_stream['simple_coll_2']]))
-        self.assertEqual(changed_ids, actual)
+        # 1 record due to fencepost querying on oplog ts
+        self.assertEqual(1, record_count_by_stream['simple_coll_1'])
+
+        final_state = menagerie.get_state(conn_id)
+
+        with get_test_connection() as client:
+            row = client.local.oplog.rs.find_one(sort=[('$natural', pymongo.DESCENDING)])
+            latest_oplog_ts = row.get('ts')
+
+        self.assertEqual(
+            (latest_oplog_ts.time, latest_oplog_ts.inc),
+            (final_state['bookmarks']['simple_db-simple_coll_1']['oplog_ts_time'],
+             final_state['bookmarks']['simple_db-simple_coll_1']['oplog_ts_inc'])
+        )
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_oplog_aged_out.py` & `tap-mongodb-3.0.0/tests/test_mongodb_oplog_aged_out.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_projection.py` & `tap-mongodb-3.0.0/tests/test_mongodb_projection.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             {
                 "projection": {"_id": 1},
                 "expected_keys": [{"_id"},
                                   {"_id", "_sdc_deleted_at"}]
             },
             {
                 "projection": {},
-                "expected_keys": [{"_id"},
+                "expected_keys": [{"_id", "string_field", "int_field"},
                                   {"_id", "_sdc_deleted_at"}]
             },
             {
                 "projection": None,
                 "expected_keys": [{"_id", "string_field", "int_field"},
                                   {"_id", "_sdc_deleted_at"}]
             },
@@ -218,14 +218,18 @@
 
 
         for stream_name in self.expected_sync_streams():
             stream_records = [x for x in messages_by_stream[stream_name]['messages'] if x.get('action') == 'upsert']
             #actual_keys = set()
 
             for record in stream_records:
+                # BUG TDL-23609. Pymongo v4.3+ returns entire document for empty projection
+                if projection_mapping['projection'] == {}:
+                    continue
+
                 self.assertIn(record['data'].keys(), projection_mapping['expected_keys'])
                 #actual_keys = actual_keys.union(set(record['data'].keys()))
 
             #self.assertTrue(actual_keys.issubset(projection_mapping['expected_keys']))
 
         self.modify_database()
 
@@ -243,14 +247,18 @@
         # verify the persisted schema was correct
         messages_by_stream = runner.get_records_from_target_output()
 
         for stream_name in self.expected_sync_streams():
             stream_records = [x for x in messages_by_stream[stream_name]['messages'] if x.get('action') == 'upsert']
             #actual_keys = set()
             for record in stream_records:
+                # BUG TDL-23609. Pymongo v4.3+ returns entire document for empty projection
+                if projection_mapping['projection'] == {}:
+                    continue
+
                 self.assertIn(record['data'].keys(), projection_mapping['expected_keys'])
                 #actual_keys = actual_keys.union(set(record['data'].keys()))
             #self.assertTrue(actual_keys.issubset(projection_mapping['expected_keys']))
 
 
     def test_run(self):
         for projection_mapping in self.projection_expected_keys_list():
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_table_reset_inc.py` & `tap-mongodb-3.0.0/tests/test_mongodb_table_reset_inc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime, timedelta
 from unittest import TestCase
 
 from mongodb_common import drop_all_collections, get_test_connection, ensure_environment_variables_set
 from tap_tester import connections, menagerie, runner
 
 RECORD_COUNT = {}
-VALID_REPLICATION_TYPES = {'datetime', 'Int64', 'float', 'int', 'str', 'Timestamp', 'UUID'}
+VALID_REPLICATION_TYPES = {'datetime', 'Int64', 'float', 'int', 'str', 'Timestamp', 'UUID', 'Binary'}
 
 def z_string_generator(size=6):
     return 'z' * size
 
 def generate_simple_coll_docs(num_docs):
     docs = []
     start_datetime = datetime(2018, 1, 1, 19, 29, 14, 578000)
```

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_table_reset_log.py` & `tap-mongodb-3.0.0/tests/test_mongodb_table_reset_log.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-2.1.3/tests/test_mongodb_views.py` & `tap-mongodb-3.0.0/tests/test_mongodb_views.py`

 * *Files identical despite different names*

