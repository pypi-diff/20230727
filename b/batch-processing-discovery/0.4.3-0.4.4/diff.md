# Comparing `tmp/batch_processing_discovery-0.4.3.tar.gz` & `tmp/batch_processing_discovery-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch_processing_discovery-0.4.3.tar", max compression
+gzip compressed data, was "batch_processing_discovery-0.4.4.tar", max compression
```

## Comparing `batch_processing_discovery-0.4.3.tar` & `batch_processing_discovery-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11349 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/LICENSE
--rw-r--r--   0        0        0     4075 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/README.md
--rw-r--r--   0        0        0      648 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/__init__.py
--rw-r--r--   0        0        0     8792 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/batch_characteristics.py
--rw-r--r--   0        0        0     2264 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/config.py
--rw-r--r--   0        0        0     5618 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/discovery.py
--rw-r--r--   0        0        0     6681 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/features_table.py
--rw-r--r--   0        0        0     4881 2023-07-04 11:18:27.861288 batch_processing_discovery-0.4.3/src/batch_processing_discovery/rules.py
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 batch_processing_discovery-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/LICENSE
+-rw-r--r--   0        0        0     4075 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/README.md
+-rw-r--r--   0        0        0      648 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/src/batch_processing_discovery/__init__.py
+-rw-r--r--   0        0        0     8792 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/src/batch_processing_discovery/batch_characteristics.py
+-rw-r--r--   0        0        0     2264 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/src/batch_processing_discovery/config.py
+-rw-r--r--   0        0        0     5618 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/src/batch_processing_discovery/discovery.py
+-rw-r--r--   0        0        0     6687 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/src/batch_processing_discovery/features_table.py
+-rw-r--r--   0        0        0     4881 2023-07-27 12:54:34.127510 batch_processing_discovery-0.4.4/src/batch_processing_discovery/rules.py
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 batch_processing_discovery-0.4.4/PKG-INFO
```

### Comparing `batch_processing_discovery-0.4.3/LICENSE` & `batch_processing_discovery-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.3/README.md` & `batch_processing_discovery-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.3/pyproject.toml` & `batch_processing_discovery-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batch-processing-discovery"
-version = "0.4.3"
+version = "0.4.4"
 description = "Python algorithm to discover, from an event log, activity instances that are executed in a batch."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "batch_processing_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `batch_processing_discovery-0.4.3/src/batch_processing_discovery/batch_characteristics.py` & `batch_processing_discovery-0.4.4/src/batch_processing_discovery/batch_characteristics.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.3/src/batch_processing_discovery/config.py` & `batch_processing_discovery-0.4.4/src/batch_processing_discovery/config.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.3/src/batch_processing_discovery/discovery.py` & `batch_processing_discovery-0.4.4/src/batch_processing_discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.3/src/batch_processing_discovery/features_table.py` & `batch_processing_discovery-0.4.4/src/batch_processing_discovery/features_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                     )
                 ]
     # Transform duration to seconds
     features_table = pd.DataFrame(data=features)
     features_table['instant'] = features_table['instant'].astype(np.int64) / 10 ** 9
     features_table['batch_ready_wt'] = features_table['batch_ready_wt'].apply(lambda t: t.total_seconds())
     features_table['batch_max_wt'] = features_table['batch_max_wt'].apply(lambda t: t.total_seconds())
-    features_table['max_cycle_time'] = features_table['max_cycle_time'].apply(lambda t: t.total_seconds())
+    # features_table['max_cycle_time'] = features_table['max_cycle_time'].apply(lambda t: t.total_seconds())
     # Return table
     return features_table
 
 
 def _get_features(
         event_log: pd.DataFrame,
         instant: pd.Timestamp,
@@ -105,29 +105,29 @@
     batch_type = batch_instance[log_ids.batch_type].iloc[0]
     activity = batch_instance[log_ids.activity].iloc[0]
     resource = batch_instance[log_ids.resource].iloc[0]
     batch_size = len(batch_instance)
     batch_ready_wt = instant - batch_instance[log_ids.enabled_time].max()
     batch_max_wt = instant - batch_instance[log_ids.enabled_time].min()
     case_ids = batch_instance[log_ids.case].unique()
-    max_cycle_time = (instant - event_log[event_log[log_ids.case].isin(case_ids)][log_ids.start_time].min())
+    # max_cycle_time = (instant - event_log[event_log[log_ids.case].isin(case_ids)][log_ids.start_time].min())
     week_day = instant.day_of_week
     # day_of_month = instant.day
     daily_hour = instant.hour
     # minute_of_day = instant.minute
     # Return the features dict
     return {
         log_ids.batch_id: batch_id,
         log_ids.batch_type: batch_type,
         log_ids.activity: activity,
         log_ids.resource: resource,
         'instant': instant,
         'batch_size': batch_size,
         'batch_ready_wt': batch_ready_wt,
         'batch_max_wt': batch_max_wt,
-        'max_cycle_time': max_cycle_time,
+        # 'max_cycle_time': max_cycle_time,
         'week_day': week_day,
         # 'day_of_month': day_of_month,
         'daily_hour': daily_hour,
         # 'minute': minute_of_day,
         'outcome': outcome
     }
```

### Comparing `batch_processing_discovery-0.4.3/src/batch_processing_discovery/rules.py` & `batch_processing_discovery-0.4.4/src/batch_processing_discovery/rules.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.3/PKG-INFO` & `batch_processing_discovery-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-processing-discovery
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python algorithm to discover, from an event log, activity instances that are executed in a batch.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

