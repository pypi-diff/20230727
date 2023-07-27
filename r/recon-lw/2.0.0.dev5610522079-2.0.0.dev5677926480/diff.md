# Comparing `tmp/recon_lw-2.0.0.dev5610522079.tar.gz` & `tmp/recon_lw-2.0.0.dev5677926480.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5610522079.tar", last modified: Thu Jul 20 11:42:04 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5677926480.tar", last modified: Thu Jul 27 07:49:00 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5610522079.tar` & `recon_lw-2.0.0.dev5677926480.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-20 11:41:39.000000 recon_lw-2.0.0.dev5610522079/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13891 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 11:42:04.000000 recon_lw-2.0.0.dev5610522079/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-20 11:41:13.000000 recon_lw-2.0.0.dev5610522079/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-27 07:48:38.000000 recon_lw-2.0.0.dev5677926480/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14283 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 07:49:00.000000 recon_lw-2.0.0.dev5677926480/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-27 07:48:16.000000 recon_lw-2.0.0.dev5677926480/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/recon_lw.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
          "parentEventId": parentId,
          "startTimestamp": {"epochSecond": int(ts.timestamp()),"nano": ts.microsecond*1000},
          "attachedMessageIds": []}
     return e
 
 
 #{"first_key_func":..., "second_key_func",... "interpret_func"}
-def execute_standalone(message_pickle_path, sessions_list, result_events_path, rules_settings_dict):
+def execute_standalone(message_pickle_path, sessions_list, result_events_path, rules_settings_dict, data_objects=None):
     events_buffer = []
     box_ts = datetime.now()
     events_saver = EventsSaver(result_events_path)
     event_sequence = {"name": "recon_lw", "stamp": str(box_ts.timestamp()), "n": 0}
     root_event = create_event("recon_lw " + box_ts.isoformat(), "Microservice", event_sequence)
 
     events_saver.save_events([root_event])
@@ -192,20 +192,23 @@
         if "collect_func" not in rule_settings:
             rule_settings["collect_func"] = collect_matcher
         if "flush_func" not in rule_settings:
             rule_settings["flush_func"] = flush_matcher
         rule_settings["init_func"](rule_settings)
 
     events_saver.save_events([r["rule_root_event"] for r in rules_settings_dict.values()])
-    if sessions_list is not None and len(sessions_list):
-        sessions_set = set(sessions_list)
-        streams = open_streams(message_pickle_path,
-                               lambda n: n[:n.rfind('_')] in sessions_set)
+    if data_objects:
+        streams = open_streams(message_pickle_path, data_objects=data_objects)
     else:
-        streams = open_streams(message_pickle_path)
+        if sessions_list is not None and len(sessions_list):
+            sessions_set = set(sessions_list)
+            streams = open_streams(message_pickle_path,
+                                lambda n: n[:n.rfind('_')] in sessions_set)
+        else:
+            streams = open_streams(message_pickle_path)
 
     message_buffer = [None]*100
     buffer_len = 100
     while len(streams)>0:
         next_batch_len = get_next_batch(streams, message_buffer, buffer_len, lambda m: m["timestamp"])
         buffer_to_process = message_buffer
         if next_batch_len < buffer_len:
@@ -322,29 +325,35 @@
         if data_filter:
             strm = strm.filter(data_filter)
         ts0 = {"epochSecond": 0, "nano": 0}
         streams.add((ts0, iter(strm), None))
     return streams
 
 
-def open_streams(streams_path, name_filter=None, expanded_messages=False):
+def open_streams(streams_path, name_filter=None, expanded_messages=False, data_objects=None):
     streams = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
-    files = listdir(streams_path)
-    for f in files:
-        if ".pickle" not in f:
-            continue
-        if name_filter is not None and not name_filter(f):
-            continue
-        data_object = Data.from_cache_file(path.join(streams_path, f))
-        if expanded_messages:
-            stream = (mm for m in data_object for mm in message_utils.expand_message(m))
-        else:
-            stream = Data.from_cache_file(path.join(streams_path, f))
-        ts0 = {"epochSecond": 0, "nano": 0}
-        streams.add((ts0, iter(stream), None))
+    
+    if data_objects:
+        for stream in data_objects:
+            ts0 = {"epochSecond": 0, "nano": 0}
+            streams.add((ts0, iter(stream), None))
+    else:
+        files = listdir(streams_path)
+        for f in files:
+            if ".pickle" not in f:
+                continue
+            if name_filter is not None and not name_filter(f):
+                continue
+            data_object = Data.from_cache_file(path.join(streams_path, f))
+            if expanded_messages:
+                stream = (mm for m in data_object for mm in message_utils.expand_message(m))
+            else:
+                stream = Data.from_cache_file(path.join(streams_path, f))
+            ts0 = {"epochSecond": 0, "nano": 0}
+            streams.add((ts0, iter(stream), None))
 
     return streams
 
 
 def get_next_batch(streams, batch, b_len, get_timestamp_func):
     batch_pos = 0
     batch_len = b_len #len(batch)
```

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5677926480/recon_lw/recon_oe_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5677926480/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/setup.py` & `recon_lw-2.0.0.dev5677926480/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5610522079/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5677926480/test/test_recon_ob.py`

 * *Files identical despite different names*

