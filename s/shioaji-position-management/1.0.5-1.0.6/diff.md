# Comparing `tmp/shioaji_position_management-1.0.5.tar.gz` & `tmp/shioaji_position_management-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_position_management-1.0.5.tar", last modified: Thu Jul 27 14:44:34 2023, max compression
+gzip compressed data, was "shioaji_position_management-1.0.6.tar", last modified: Thu Jul 27 18:34:17 2023, max compression
```

## Comparing `shioaji_position_management-1.0.5.tar` & `shioaji_position_management-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.5/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2692 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2084 2023-07-27 14:44:17.000000 shioaji_position_management-1.0.5/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.5/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.577598 shioaji_position_management-1.0.5/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.585598 shioaji_position_management-1.0.5/src/shioaji_position_management/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.5/src/shioaji_position_management/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3163 2023-07-27 14:43:59.000000 shioaji_position_management-1.0.5/src/shioaji_position_management/shioaji_position_management.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2692 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 18:34:17.784328 shioaji_position_management-1.0.6/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.6/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2748 2023-07-27 18:34:17.784328 shioaji_position_management-1.0.6/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2140 2023-07-27 18:34:01.000000 shioaji_position_management-1.0.6/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.6/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-27 18:34:17.788328 shioaji_position_management-1.0.6/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 18:34:17.756328 shioaji_position_management-1.0.6/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 18:34:17.768328 shioaji_position_management-1.0.6/src/shioaji_position_management/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.6/src/shioaji_position_management/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4094 2023-07-27 18:33:29.000000 shioaji_position_management-1.0.6/src/shioaji_position_management/shioaji_position_management.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 18:34:17.780328 shioaji_position_management-1.0.6/src/shioaji_position_management.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2748 2023-07-27 18:34:17.000000 shioaji_position_management-1.0.6/src/shioaji_position_management.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-27 18:34:17.000000 shioaji_position_management-1.0.6/src/shioaji_position_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-27 18:34:17.000000 shioaji_position_management-1.0.6/src/shioaji_position_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-27 18:34:17.000000 shioaji_position_management-1.0.6/src/shioaji_position_management.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-27 18:34:17.000000 shioaji_position_management-1.0.6/src/shioaji_position_management.egg-info/top_level.txt
```

### Comparing `shioaji_position_management-1.0.5/LICENSE` & `shioaji_position_management-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shioaji_position_management-1.0.5/PKG-INFO` & `shioaji_position_management-1.0.6/src/shioaji_position_management.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shioaji_position_management
-Version: 1.0.5
+Name: shioaji-position-management
+Version: 1.0.6
 Summary: An Extensions help you trading with Sinopac shioaji
 Home-page: https://github.com/NickLin910221/shioaji_position_management
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Position_Management/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,16 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
-- v1.0.5 (2023/7/27) fix some bugs about order
+- v1.0.6 (2023/7/28) Adjust the log of callback message
+- v1.0.5 (2023/7/27) Fix some bugs about order
 - v1.0.4
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

### Comparing `shioaji_position_management-1.0.5/README.md` & `shioaji_position_management-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
-- v1.0.5 (2023/7/27) fix some bugs about order
+- v1.0.6 (2023/7/28) Adjust the log of callback message
+- v1.0.5 (2023/7/27) Fix some bugs about order
 - v1.0.4
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

### Comparing `shioaji_position_management-1.0.5/setup.cfg` & `shioaji_position_management-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_position_management
-version = 1.0.5
+version = 1.0.6
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you trading with Sinopac shioaji
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/shioaji_position_management
```

### Comparing `shioaji_position_management-1.0.5/src/shioaji_position_management/shioaji_position_management.py` & `shioaji_position_management-1.0.6/src/shioaji_position_management/shioaji_position_management.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,16 +21,25 @@
 
         logger.add(f"./shioaji_position_management_{datetime.datetime.today().strftime('%Y-%m-%d')}.log", encoding="utf-8", enqueue=True)
         logger.info(f"-----Seperate Line-----")
         logger.info(f"shioaji_position_management Start at {datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}")
         logger.info(f"Start monitoring {self.acc}")
 
     def cb(self, stat, msg):
-        logger.info(f"Callback status {stat}")
-        logger.info(f"msg {msg}")
+        if stat in [sj.constant.OrderState.FuturesOrder, sj.constant.OrderState.StockOrder]:
+            logger.info(f"{stat}")
+            logger.info(f"Operation : {msg['operation']['op_type']}, Operation_Code : {msg['operation']['op_msg']}, Operation_Msg : {msg['operation']['op_msg']}")
+            logger.info(f"ID : {msg['order']['id']}, seqno : {msg['order']['seqno']}, ordno {msg['order']['ordno']}")
+            logger.info(f"{msg['order']['action']} {msg['order']['quantity']} {msg['contract']['code']}@{msg['order']['price']}, ts : {datetime.datetime.fromtimestamp(msg['status']['exchange_ts'])}")
+        # TODO : sj.constant.StockDeal
+        elif stat in [sj.constant.OrderState.FuturesDeal]:
+            logger.info(f"{stat}")
+            logger.info(f"ID : {msg['trade_id']}, seqno : {msg['seqno']}, ordno {msg['ordno']}")
+            logger.info(f"{msg['action']} {msg['quantity']} {msg['code']}@{msg['price']}, ts : {datetime.datetime.fromtimestamp(msg['ts'])}")
+        ## Manage Position    
         if "DEAL" in stat:
             self.future.append(msg)
 
     def close_all_position(self):
         for p in self.future:
             self.order(self, self.api.Contracts.Futures.MXF[p.code], "S" if p.action == "Buy" else "B", p.price, p.quantity, "MKT", "IOC", "Auto")
```

### Comparing `shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/PKG-INFO` & `shioaji_position_management-1.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shioaji-position-management
-Version: 1.0.5
+Name: shioaji_position_management
+Version: 1.0.6
 Summary: An Extensions help you trading with Sinopac shioaji
 Home-page: https://github.com/NickLin910221/shioaji_position_management
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Position_Management/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,16 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
-- v1.0.5 (2023/7/27) fix some bugs about order
+- v1.0.6 (2023/7/28) Adjust the log of callback message
+- v1.0.5 (2023/7/27) Fix some bugs about order
 - v1.0.4
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

