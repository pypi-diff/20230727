# Comparing `tmp/tap-pendo-0.6.2.tar.gz` & `tmp/tap-pendo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-pendo-0.6.2.tar", last modified: Mon Apr 10 13:43:38 2023, max compression
+gzip compressed data, was "tap-pendo-1.0.0.tar", last modified: Thu Jul 27 15:08:44 2023, max compression
```

## Comparing `tap-pendo-0.6.2.tar` & `tap-pendo-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.070166 tap-pendo-0.6.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-04-10 13:43:38.070166 tap-pendo-0.6.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15851 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-10 13:43:38.070166 tap-pendo-0.6.2/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      916 2023-04-10 13:35:39.000000 tap-pendo-0.6.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.054166 tap-pendo-0.6.2/tap_pendo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5901 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5091 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.066166 tap-pendo-0.6.2/tap_pendo/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      838 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/feature_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4166 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/features.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1598 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/guide_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5944 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/guides.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/metadata_accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/metadata_visitors.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/page_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3657 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/pages.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/poll_events.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.066166 tap-pendo-0.6.2/tap_pendo/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/shared/metadata.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/track_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2327 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/track_types.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1262 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/visitor_history.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1931 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/schemas/visitors.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58745 2023-04-10 13:35:39.000000 tap-pendo-0.6.2/tap_pendo/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4201 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-04-05 10:03:46.000000 tap-pendo-0.6.2/tap_pendo/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:43:38.054166 tap-pendo-0.6.2/tap_pendo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-10 13:43:38.000000 tap-pendo-0.6.2/tap_pendo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16198 2023-07-27 14:41:26.000000 tap-pendo-1.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      916 2023-07-27 15:05:22.000000 tap-pendo-1.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.422115 tap-pendo-1.0.0/tap_pendo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6721 2023-07-27 08:24:30.000000 tap-pendo-1.0.0/tap_pendo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5091 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/tap_pendo/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      922 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      838 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/feature_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4222 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/features.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-07-27 14:41:26.000000 tap-pendo-1.0.0/tap_pendo/schemas/guide_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6000 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/guides.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/metadata_accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/metadata_visitors.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2023-07-27 08:18:39.000000 tap-pendo-1.0.0/tap_pendo/schemas/page_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/pages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1392 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/poll_events.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.426115 tap-pendo-1.0.0/tap_pendo/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/shared/metadata.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/track_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2383 2023-07-27 07:41:52.000000 tap-pendo-1.0.0/tap_pendo/schemas/track_types.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1262 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/visitor_history.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1931 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/schemas/visitors.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    59547 2023-07-27 14:41:26.000000 tap-pendo-1.0.0/tap_pendo/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4201 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-04-05 10:03:46.000000 tap-pendo-1.0.0/tap_pendo/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 15:08:44.422115 tap-pendo-1.0.0/tap_pendo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-07-27 15:08:44.000000 tap-pendo-1.0.0/tap_pendo.egg-info/top_level.txt
```

### Comparing `tap-pendo-0.6.2/LICENSE` & `tap-pendo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/README.md` & `tap-pendo-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -101,60 +101,60 @@
   - Bookmark: `modified_ts` (Max from `ts` or `lastTs`)
 - Transformations: Camel to snake case.
 
 **[feature_events](https://developers.pendo.io/docs/?bash#get-an-account-by-id)**
 
 - US Subscription Endpoint: [https://app.pendo.io/api/v1/aggregation](https://app.pendo.io/api/v1/aggregation)
 - EU Subscription Endpoint: [https://app.eu.pendo.io/api/v1/aggregation](https://app.eu.pendo.io/api/v1/aggregation)
-- Primary key fields: `visitor_id`, `account_id`, `server`, `remote_ip`
+- Primary key fields: `feature_id`, `visitor_id`, `account_id`, `remote_ip`, `user_agent`, `day` or `hour`
 - Replication strategy: INCREMENTAL (query filtered)
   - Bookmark: `day` or `hour`
 - Transformations: Camel to snake case.
 
 **[events](https://developers.pendo.io/docs/?bash#get-an-account-by-id)**
 
 - US Subscription Endpoint: [https://app.pendo.io/api/v1/aggregation](https://app.pendo.io/api/v1/aggregation)
 - EU Subscription Endpoint: [https://app.eu.pendo.io/api/v1/aggregation](https://app.eu.pendo.io/api/v1/aggregation)
-- Primary key fields: `visitor_id`, `account_id`, `server`, `remote_ip`
+- Primary key fields: `visitor_id`, `account_id`, `remote_ip`, `user_agent`, `day` or `hour`
 - Replication strategy: INCREMENTAL (query filtered)
   - Bookmark: `day` or `hour`
 - Transformations: Camel to snake case.
 
 **[page_events](https://developers.pendo.io/docs/?bash#get-an-account-by-id)**
 
 - US Subscription Endpoint: [https://app.pendo.io/api/v1/aggregation](https://app.pendo.io/api/v1/aggregation)
 - EU Subscription Endpoint: [https://app.eu.pendo.io/api/v1/aggregation](https://app.eu.pendo.io/api/v1/aggregation)
-- Primary key fields: `visitor_id`, `account_id`, `server`, `remote_ip`
+- Primary key fields: `page_id`, `visitor_id`, `account_id`, `remote_ip`, `user_agent`, `day` or `hour`
 - Replication strategy: INCREMENTAL (query filtered)
   - Bookmark: `day` or `hour`
 - Transformations: Camel to snake case.
 
 **[guide_events](https://developers.pendo.io/docs/?bash#get-an-account-by-id)**
 
 - US Subscription Endpoint: [https://app.pendo.io/api/v1/aggregation](https://app.pendo.io/api/v1/aggregation)
 - EU Subscription Endpoint: [https://app.eu.pendo.io/api/v1/aggregation](https://app.eu.pendo.io/api/v1/aggregation)
-- Primary key fields: `visitor_id`, `account_id`, `server`, `remote_ip`
+- Primary key fields: `guide_id`, `guide_step_id`, `visitor_id`, `type`, `account_id`, `browser_time`, `url`
 - Replication strategy: INCREMENTAL (query filtered)
   - Bookmark: `browserTime`
 - Transformations: Camel to snake case.
 
 **[poll_events](https://developers.pendo.io/docs/?bash#get-an-account-by-id)**
 
 - US Subscription Endpoint: [https://app.pendo.io/api/v1/aggregation](https://app.pendo.io/api/v1/aggregation)
 - EU Subscription Endpoint: [https://app.eu.pendo.io/api/v1/aggregation](https://app.eu.pendo.io/api/v1/aggregation)
-- Primary key fields: `visitor_id`, `account_id`, `server`, `remote_ip`
+- Primary key fields: `visitor_id`, `account_id`, `poll_id`, `browser_time`
 - Replication strategy: INCREMENTAL (query filtered)
   - Bookmark: `browserTime`
 - Transformations: Camel to snake case.
 
 **[track_events](https://developers.pendo.io/docs/?bash#get-an-account-by-id)**
 
 - US Subscription Endpoint: [https://app.pendo.io/api/v1/aggregation](https://app.pendo.io/api/v1/aggregation)
 - EU Subscription Endpoint: [https://app.eu.pendo.io/api/v1/aggregation](https://app.eu.pendo.io/api/v1/aggregation)
-- Primary key fields: `visitor_id`, `account_id`, `server`, `remote_ip`
+- Primary key fields: `track_type_id`, `visitor_id`, `account_id`, `remote_ip`, `user_agent`, `day` or `hour`
 - Replication strategy: INCREMENTAL (query filtered)
   - Bookmark: `day` or `hour`
 - Transformations: Camel to snake case.
 
 **[guides](https://developers.pendo.io/docs/?bash#entities)**
 
 - US Subscription Endpoint: [https://app.pendo.io/api/v1/aggregation](https://app.pendo.io/api/v1/aggregation)
@@ -258,31 +258,31 @@
    - [jsonlines](https://jsonlines.readthedocs.io/en/latest/)
 
 3. Create your tap's `config.json` file. The tap config file for this tap should include these entries:
 
    - `start_date` - the default value to use if no bookmark exists for an endpoint (rfc3339 date string)
    - `x_pendo_integration_key` (string, `ABCdef123`): an integration key from Pendo.
    - `period` (string, `ABCdef123`): `dayRange` or `hourRange`
-   - `lookback_window` (integer, 10): For event objects. Default: 0 days
-   - `request_timeout` (integer, 300) For passing timeout to the request. Default: 300 seconds
+   - `lookback_window` (integer): 10 (For event objects. Default: 0)
+   - `request_timeout` (integer): 300 (For passing timeout to the request. Default: 300)
    - `record_limit` (integer, 100000): maximum number of records Pendo API can retrieve in a single request. Default: 100000 records
+   - `app_ids` (string, `8877665523, 1234545`): (comma seperated appIDs. If this parameter is not provided, then the data will be collected from all the apps)
 
-   ```
    Note: It is important to set `record_limit` parameter to an appropriate value, as selecting a smaller value may have a negative effect on the Pendo API's performance, while a larger value may result in connection errors, request timeouts, or memory overflows.
    ```
-
    ```json
    {
      "x_pendo_integration_key": "YOUR_INTEGRATION_KEY",
      "start_date": "2020-09-18T00:00:00Z",
      "period": "dayRange",
      "lookback_window": 10,
      "request_timeout": 300,
      "record_limit": 100000,
-     "include_anonymous_visitors": "true"
+     "include_anonymous_visitors": "true",
+     "app_ids": "1234545, 8877665523"
    }
    ```
 
 4. Run the Tap in Discovery Mode
    This creates a catalog.json for selecting objects/fields to integrate:
 
    ```bash
```

### Comparing `tap-pendo-0.6.2/setup.py` & `tap-pendo-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-pendo",
-    version="0.6.2",
+    version="1.0.0",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="https://github.com/singer-io/tap-pendo",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_pendo"],
     install_requires=[
         'singer-python==5.13.0',
```

### Comparing `tap-pendo-0.6.2/tap_pendo/__init__.py` & `tap-pendo-1.0.0/tap_pendo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -148,19 +148,40 @@
             counter_value = sync_full_table(state, instance)
         singer.write_state(state)
         LOGGER.info("Stream %s: Completed sync (%s rows)", stream_id, counter_value)
         update_currently_syncing(state, None)
         singer.write_state(state)
     LOGGER.info("Finished sync")
 
+# To check that given number is numeric or not
+def filter_app_ids(config):
+    # reason to use expandAppIds
+    # https://support.pendo.io/hc/en-us/community/posts/360078029732-How-to-retrieve-all-application-data-using-Pendo-API-through-Python
+    app_ids = config.get("app_ids") or "expandAppIds(\"*\")"
+
+    invalid_app_ids = []
+    if app_ids != "expandAppIds(\"*\")":
+        app_ids = [app_id.strip() for app_id in app_ids.split(",")]
+        for app_id in app_ids:
+            try:
+                int(app_id)
+            except ValueError:
+                invalid_app_ids.append(app_id)
+        if invalid_app_ids:
+            raise Exception(f"Invalid appIDs provided during the configuration:{invalid_app_ids}")
+    config["app_ids"] = app_ids
+    return config
+
+
 @utils.handle_top_exception(LOGGER)
 def main():
 
     # Parse command line arguments
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
+    args.config = filter_app_ids(args.config)
 
     if args.discover:
         do_discover(args.config)
     elif args.catalog:
         state = args.state
         sync(args.config, state, args.catalog)
```

### Comparing `tap-pendo-0.6.2/tap_pendo/discover.py` & `tap-pendo-1.0.0/tap_pendo/discover.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/accounts.json` & `tap-pendo-1.0.0/tap_pendo/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/events.json` & `tap-pendo-1.0.0/tap_pendo/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/feature_events.json` & `tap-pendo-1.0.0/tap_pendo/schemas/feature_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/features.json` & `tap-pendo-1.0.0/tap_pendo/schemas/features.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'properties'": "{'app_id': OrderedDict([('type', ['null', 'number'])])}"}*

```diff
@@ -1,9 +1,15 @@
 {
     "properties": {
+        "app_id": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "color": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "created_at": {
```

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/guide_events.json` & `tap-pendo-1.0.0/tap_pendo/schemas/poll_events.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4,47 +4,59 @@
     "properties": {
         "app_id": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "account_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "account_ids": {
             "anyOf": [
                 {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
                 },
                 {
                     "type": "null"
                 }
             ]
         },
-        "browser_time": {
+        "poll_id": {
             "type": [
                 "null",
                 "string"
-            ],
-            "format": "date-time"
+            ]
         },
-        "country": {
+        "guide_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "type": {
+        "browser_time": {
+            "type": [
+                "null",
+                "string"
+            ],
+            "format": "date-time"
+        },
+        "country": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "guide_id": {
+        "type": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "latitude": {
             "type": [
@@ -60,20 +72,14 @@
         },
         "longitude": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "poll_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "region": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "remote_ip": {
@@ -96,20 +102,14 @@
         },
         "visitor_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "account_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "poll_response": {
             "type": [
                 "null",
                 "string"
             ]
         }
     }
```

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/guides.json` & `tap-pendo-1.0.0/tap_pendo/schemas/guides.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'properties'": "{'app_id': OrderedDict([('type', ['null', 'number'])])}"}*

```diff
@@ -1,9 +1,15 @@
 {
     "properties": {
+        "app_id": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "attributes": {
             "properties": {
                 "badge": {
                     "properties": {
                         "can_change_badge_color": {
                             "type": [
                                 "null",
```

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/metadata_accounts.json` & `tap-pendo-1.0.0/tap_pendo/schemas/metadata_accounts.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/metadata_visitors.json` & `tap-pendo-1.0.0/tap_pendo/schemas/metadata_visitors.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/page_events.json` & `tap-pendo-1.0.0/tap_pendo/schemas/page_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/pages.json` & `tap-pendo-1.0.0/tap_pendo/schemas/pages.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'properties'": "{'app_id': OrderedDict([('type', ['null', 'number'])])}"}*

```diff
@@ -1,10 +1,16 @@
 {
     "additional_properties": false,
     "properties": {
+        "app_id": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "color": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "created_at": {
```

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/poll_events.json` & `tap-pendo-1.0.0/tap_pendo/schemas/guide_events.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'properties'": "{'app_id': OrderedDict([('type', ['null', 'number'])]), 'guide_step_id': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'url': OrderedDict([('type', "*

 * *                 "['null', 'string'])])}"}*

```diff
@@ -16,14 +16,20 @@
                     "type": "array"
                 },
                 {
                     "type": "null"
                 }
             ]
         },
+        "app_id": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "browser_time": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
@@ -35,14 +41,20 @@
         },
         "guide_id": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "guide_step_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "latitude": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "load_time": {
@@ -89,14 +101,20 @@
         },
         "type": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "user_agent": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "visitor_id": {
```

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/shared/metadata.json` & `tap-pendo-1.0.0/tap_pendo/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/track_events.json` & `tap-pendo-1.0.0/tap_pendo/schemas/track_events.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/track_types.json` & `tap-pendo-1.0.0/tap_pendo/schemas/track_types.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888888888888889%*

 * *Differences: {"'properties'": "{'app_id': OrderedDict([('type', ['null', 'number'])])}"}*

```diff
@@ -1,10 +1,16 @@
 {
     "additional_properties": false,
     "properties": {
+        "app_id": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "color": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "created_at": {
```

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/visitor_history.json` & `tap-pendo-1.0.0/tap_pendo/schemas/visitor_history.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/schemas/visitors.json` & `tap-pendo-1.0.0/tap_pendo/schemas/visitors.json`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/streams.py` & `tap-pendo-1.0.0/tap_pendo/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -746,15 +746,15 @@
             # which flush out during sync_substream call above
             stream_response = self.request(self.name, json=self.get_body()) or []
 
         return (self.stream, stream_response), False
 
 class EventsBase(Stream):
     DATE_WINDOW_SIZE = 1
-    key_properties = ['visitor_id', 'account_id', 'server', 'remote_ip']
+    key_properties = ['visitor_id', 'account_id', 'remote_ip']
     replication_method = "INCREMENTAL"
 
     def __init__(self, config):
         super().__init__(config=config)
         self.config = config
         self.period = config.get('period')
         self.replication_key = "day" if self.period == 'dayRange' else "hour"
@@ -886,15 +886,15 @@
             "response": {
                 "mimeType": "application/json"
             },
             "request": {
                 "name": "all-accounts",
                 "pipeline": [{
                     "source": {
-                        "accounts": None
+                        "accounts": {"appId": self.config["app_ids"]}
                     },
                 }, {
                     "sort": ["metadata.auto.lastupdated"]
                 }, {
                     "filter": "metadata.auto.lastupdated>=1"
                 }, {
                     "limit": self.record_limit
@@ -928,15 +928,15 @@
                 "mimeType": "application/json"
             },
             "request": {
                 "name":
                 "all-features",
                 "pipeline": [{
                     "source": {
-                        "features": None
+                        "features": {"appId": self.config["app_ids"]}
                     }
                 }, {
                     "sort": [f"{self.replication_key}"]
                 }, {
                     "limit": self.record_limit
                 }],
                 "requestId":
@@ -944,33 +944,38 @@
             }
         }
 
 
 class FeatureEvents(EventsBase):
     name = "feature_events"
     replication_method = "INCREMENTAL"
-    key_properties = ['visitor_id', 'account_id', 'server', 'remote_ip']
+    key_properties = ['feature_id', 'visitor_id', 'account_id', 'remote_ip', 'user_agent']
+
+    def __init__(self, config):
+        super().__init__(config=config)
+        self.key_properties.append("day" if self.period == 'dayRange' else "hour")
 
     def get_body(self, key_id, period, first):
         body = super().get_body(key_id, period, first)
-        body['request']['pipeline'][0]['source'].update({"featureEvents": {"featureId": key_id,}})
+        body['request']['pipeline'][0]['source'].update({"featureEvents": {"featureId": key_id}})
         return body
 
 
 class Events(EventsBase):
     name = "events"
     DATE_WINDOW_SIZE = 1
-    key_properties = ['visitor_id', 'account_id', 'server', 'remote_ip']
+    key_properties = ['visitor_id', 'account_id', 'remote_ip', 'user_agent']
     replication_method = "INCREMENTAL"
 
     def __init__(self, config):
         super().__init__(config=config)
         self.config = config
         self.period = config.get('period')
         self.replication_key = "day" if self.period == 'dayRange' else "hour"
+        self.key_properties.append(self.replication_key)
 
     def get_events(self, window_start_date, state, bookmark_dttm):
         # initialize start date as max bookmark
         max_bookmark = bookmark_dttm
         # Get period type from config and make request for event's data
         period = self.config.get('period')
         # date format to filter
@@ -1028,59 +1033,61 @@
                 break
 
     def transform(self, record):
         return humps.decamelize(record)
 
     def get_body(self, key_id, period, first):
         body = super().get_body(key_id, period, first)
-        body['request']['pipeline'][0]['source'].update({"events": None})
+        body['request']['pipeline'][0]['source'].update({"events": {"appId": self.config["app_ids"]}})
         return body
 
 
-
 class PollEvents(EventsBase):
     replication_method = "INCREMENTAL"
     name = "poll_events"
-    key_properties = ['visitor_id', 'account_id', 'server_name', 'remote_ip']
+    key_properties = ['visitor_id', 'account_id', 'poll_id', 'browser_time']
 
     def __init__(self, config):
         super().__init__(config=config)
         self.config = config
         self.period = config.get('period')
         self.replication_key = 'browser_time'
 
     def get_body(self, key_id, period, first):
         body = super().get_body(key_id, period, first)
-        body['request']['pipeline'][0]['source'].update({"pollEvents": None})
+        body['request']['pipeline'][0]['source'].update({"pollEvents": {"appId": self.config["app_ids"]}})
         return body
 
 
 class TrackEvents(EventsBase):
     replication_method = "INCREMENTAL"
     name = "track_events"
-    key_properties = ['visitor_id', 'account_id', 'server', 'remote_ip']
+    key_properties = ['track_type_id', 'visitor_id', 'account_id', 'remote_ip', 'user_agent']
 
+    def __init__(self, config):
+        super().__init__(config=config)
+        self.key_properties.append("day" if self.period == 'dayRange' else "hour")
 
     def get_body(self, key_id, period, first):
         body = super().get_body(key_id, period, first)
-        body['request']['pipeline'][0]['source'].update({"trackEvents": {"trackTypeId": key_id,}})
+        body['request']['pipeline'][0]['source'].update({"trackEvents": {"trackTypeId": key_id}})
         return body
 
 class GuideEvents(EventsBase):
     replication_method = "INCREMENTAL"
     name = "guide_events"
-    key_properties = ['visitor_id', 'account_id', 'server_name', 'remote_ip']
+    key_properties = ['guide_id', 'guide_step_id', 'visitor_id', 'type', 'account_id', 'browser_time', 'url']
 
     def __init__(self, config):
         super().__init__(config=config)
         self.replication_key = 'browser_time'
 
     def get_body(self, key_id, period, first):
         body = super().get_body(key_id, period, first)
-        body['request']['pipeline'][0]['source'].update({"guideEvents": {"guideId": key_id,}})
+        body['request']['pipeline'][0]['source'].update({"guideEvents": {"guideId": key_id}})
         return body
 
 
 class TrackTypes(Stream):
     name = "track_types"
     replication_method = "INCREMENTAL"
     replication_key = "lastUpdatedAt"
@@ -1090,15 +1097,15 @@
             "response": {
                 "mimeType": "application/json"
             },
             "request": {
                 "name": "all-track-types",
                 "pipeline": [{
                     "source": {
-                        "trackTypes": None
+                        "trackTypes": {"appId": self.config["app_ids"]}
                     }
                 }, {
                     "sort": [f"{self.replication_key}"]
                 }, {
                     "limit": self.record_limit
                 }],
                 "requestId": "all-track-types"
@@ -1117,15 +1124,15 @@
                 "mimeType": "application/json"
             },
             "request": {
                 "name":
                 "all-guides",
                 "pipeline": [{
                     "source": {
-                        "guides": None
+                        "guides": {"appId": self.config["app_ids"]}
                     }
                 }, {
                     "sort": [f"{self.replication_key}"]
                 }, {
                     "limit": self.record_limit
                 }],
                 "requestId":
@@ -1145,15 +1152,15 @@
                 "mimeType": "application/json"
             },
             "request": {
                 "name":
                 "all-pages",
                 "pipeline": [{
                     "source": {
-                        "pages": None
+                        "pages": {"appId": self.config["app_ids"]}
                     }
                 }, {
                     "sort": [f"{self.replication_key}"]
                 }, {
                     "limit": self.record_limit
                 }],
                 "requestId":
@@ -1161,19 +1168,23 @@
             }
         }
 
 
 class PageEvents(EventsBase):
     name = "page_events"
     replication_method = "INCREMENTAL"
-    key_properties = ['visitor_id', 'account_id', 'server', 'remote_ip']
+    key_properties = ['page_id', 'visitor_id', 'account_id', 'remote_ip', 'user_agent',]
+
+    def __init__(self, config):
+        super().__init__(config=config)
+        self.key_properties.append("day" if self.period == 'dayRange' else "hour")
 
     def get_body(self, key_id, period, first):
         body = super().get_body(key_id, period, first)
-        body['request']['pipeline'][0]['source'].update({"pageEvents": {"pageId": key_id,}})
+        body['request']['pipeline'][0]['source'].update({"pageEvents": {"pageId": key_id}})
         return body
 
 
 class Reports(Stream):
     name = "reports"
     replication_method = "INCREMENTAL"
     replication_key = "lastUpdatedAt"
```

### Comparing `tap-pendo-0.6.2/tap_pendo/sync.py` & `tap-pendo-1.0.0/tap_pendo/sync.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo/utils.py` & `tap-pendo-1.0.0/tap_pendo/utils.py`

 * *Files identical despite different names*

### Comparing `tap-pendo-0.6.2/tap_pendo.egg-info/SOURCES.txt` & `tap-pendo-1.0.0/tap_pendo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

