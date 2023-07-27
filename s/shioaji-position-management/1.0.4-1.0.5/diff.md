# Comparing `tmp/shioaji_position_management-1.0.4.tar.gz` & `tmp/shioaji_position_management-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_position_management-1.0.4.tar", last modified: Thu Jul 27 14:41:16 2023, max compression
+gzip compressed data, was "shioaji_position_management-1.0.5.tar", last modified: Thu Jul 27 14:44:34 2023, max compression
```

## Comparing `shioaji_position_management-1.0.4.tar` & `shioaji_position_management-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.959315 shioaji_position_management-1.0.4/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.4/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2683 2023-07-27 14:41:16.959315 shioaji_position_management-1.0.4/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2075 2023-07-27 14:40:37.000000 shioaji_position_management-1.0.4/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.4/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-27 14:41:16.963315 shioaji_position_management-1.0.4/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.943315 shioaji_position_management-1.0.4/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.951315 shioaji_position_management-1.0.4/src/shioaji_position_management/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.4/src/shioaji_position_management/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3133 2023-07-27 14:40:55.000000 shioaji_position_management-1.0.4/src/shioaji_position_management/shioaji_position_management.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.959315 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2683 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.5/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2692 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2084 2023-07-27 14:44:17.000000 shioaji_position_management-1.0.5/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.5/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.577598 shioaji_position_management-1.0.5/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.585598 shioaji_position_management-1.0.5/src/shioaji_position_management/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.5/src/shioaji_position_management/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3163 2023-07-27 14:43:59.000000 shioaji_position_management-1.0.5/src/shioaji_position_management/shioaji_position_management.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:44:34.593598 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2692 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-27 14:44:34.000000 shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/top_level.txt
```

### Comparing `shioaji_position_management-1.0.4/LICENSE` & `shioaji_position_management-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shioaji_position_management-1.0.4/PKG-INFO` & `shioaji_position_management-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji_position_management
-Version: 1.0.4
+Version: 1.0.5
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
-- v1.0.4 (2023/7/27) fix some bugs about order
+- v1.0.5 (2023/7/27) fix some bugs about order
+- v1.0.4
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

### Comparing `shioaji_position_management-1.0.4/README.md` & `shioaji_position_management-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
-- v1.0.4 (2023/7/27) fix some bugs about order
+- v1.0.5 (2023/7/27) fix some bugs about order
+- v1.0.4
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

### Comparing `shioaji_position_management-1.0.4/setup.cfg` & `shioaji_position_management-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_position_management
-version = 1.0.4
+version = 1.0.5
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you trading with Sinopac shioaji
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/shioaji_position_management
```

### Comparing `shioaji_position_management-1.0.4/src/shioaji_position_management/shioaji_position_management.py` & `shioaji_position_management-1.0.5/src/shioaji_position_management/shioaji_position_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 class shioaji_position_management:
     __slots__ = ["api", "stock", "future", "option", "ordering", "acc", "logger"]
 
     def __init__(self, api, acc):
         self.api = api
         assert len(api.list_accounts()) > 0
-        self.acc = api.list_accounts()[0] 
-        for account in api.list_accounts():
+        self.acc = self.api.list_accounts()[0] 
+        for account in self.api.list_accounts():
             if account["broker_id"] + "-" + account["account_id"] == acc:
                 self.acc = account
-        api.set_order_callback(self.cb)
+        self.api.set_order_callback(self.cb)
 
         self.stock = []
         self.future = []
         self.option = []
         self.ordering = []
 
         logger.add(f"./shioaji_position_management_{datetime.datetime.today().strftime('%Y-%m-%d')}.log", encoding="utf-8", enqueue=True)
@@ -28,15 +28,15 @@
         logger.info(f"Callback status {stat}")
         logger.info(f"msg {msg}")
         if "DEAL" in stat:
             self.future.append(msg)
 
     def close_all_position(self):
         for p in self.future:
-            self.order(self, api.Contracts.Futures.MXF[p.code], "S" if p.action == "Buy" else "B", p.price, p.quantity, "MKT", "IOC", "Auto")
+            self.order(self, self.api.Contracts.Futures.MXF[p.code], "S" if p.action == "Buy" else "B", p.price, p.quantity, "MKT", "IOC", "Auto")
 
     def order(self, obj, action, price, qty, price_type, order_type, oc_type):
         assert action in ["B", "Buy", "BUY", "L", "Long", "LONG", "S", "Sell", "SELL", "Short", "SHORT"]
         if action in ["B", "Buy", "BUY", "L", "Long", "LONG"]:
             action = sj.constant.Action.Buy
         elif action in ["S", "Sell", "SELL", "Short", "SHORT"]:
             action = sj.constant.Action.Sell
@@ -63,17 +63,17 @@
         elif oc_type == "New":
             oc_type = sj.constant.FuturesOCType.New
         elif oc_type == "Cover":
             oc_type = sj.constant.FuturesOCType.Cover
         elif oc_type == "DayTrade":
             oc_type = sj.constant.FuturesOCType.DayTrade
 
-        order = api.Order(
+        order = self.api.Order(
                 action = action,
                 price = price,
                 quantity = qty,
                 price_type = price_type,
                 order_type = order_type, 
                 octype = oc_type,
                 account = self.acc
             )
-        trade = api.place_order(obj, order)
+        trade = self.api.place_order(obj, order)
```

### Comparing `shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/PKG-INFO` & `shioaji_position_management-1.0.5/src/shioaji_position_management.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji-position-management
-Version: 1.0.4
+Version: 1.0.5
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
-- v1.0.4 (2023/7/27) fix some bugs about order
+- v1.0.5 (2023/7/27) fix some bugs about order
+- v1.0.4
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

