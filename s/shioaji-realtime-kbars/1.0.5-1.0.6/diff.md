# Comparing `tmp/shioaji_realtime_kbars-1.0.5.tar.gz` & `tmp/shioaji_realtime_kbars-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_realtime_kbars-1.0.5.tar", last modified: Tue Jul 18 16:47:37 2023, max compression
+gzip compressed data, was "shioaji_realtime_kbars-1.0.6.tar", last modified: Thu Jul 27 16:46:11 2023, max compression
```

## Comparing `shioaji_realtime_kbars-1.0.5.tar` & `shioaji_realtime_kbars-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.5/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5851 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5257 2023-07-18 16:47:01.000000 shioaji_realtime_kbars-1.0.5/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.5/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      764 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.592853 shioaji_realtime_kbars-1.0.5/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.596853 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5398 2023-07-18 16:35:18.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5851 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       21 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 16:46:11.971093 shioaji_realtime_kbars-1.0.6/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.6/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5791 2023-07-27 16:46:11.971093 shioaji_realtime_kbars-1.0.6/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5197 2023-07-27 16:45:54.000000 shioaji_realtime_kbars-1.0.6/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.6/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      764 2023-07-27 16:46:11.975093 shioaji_realtime_kbars-1.0.6/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 16:46:11.967093 shioaji_realtime_kbars-1.0.6/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 16:46:11.967093 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5368 2023-07-27 16:45:29.000000 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 16:46:11.971093 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5791 2023-07-27 16:46:11.000000 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-07-27 16:46:11.000000 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-27 16:46:11.000000 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       21 2023-07-27 16:46:11.000000 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-07-27 16:46:11.000000 shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars.egg-info/top_level.txt
```

### Comparing `shioaji_realtime_kbars-1.0.5/PKG-INFO` & `shioaji_realtime_kbars-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji_realtime_kbars
-Version: 1.0.5
+Version: 1.0.6
 Summary: An Extensions help you streaming with real-time data
 Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -116,22 +116,24 @@
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
 ### Callback funtion
+```
 shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe?
 
 Signature:
 shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe(
     contract: List[Union[shioaji.contracts.Option, shioaji.contracts.Future, shioaji.contracts.Stock, shioaji.contracts.Index]],
     last_days: int = 0,
     cb: Any = List[[callback_function, period]]
 ) -> None
+```
 
 ### Example
 If you want to clearly write your strategy. You can refer to example
 
 ```
 def strategy(period, kbars):
     print(period)
@@ -159,24 +161,20 @@
         Contracts.update(tick, "fop")
 
     Event().wait()
 ```
 
 
 ## Version
-### v1.0.5 (2023/7/19)
-#### * Add callback function
-### v1.0.4 (2023/7/17)
-#### * Fix resampling will have some NaN rows
-### v1.0.3 (2023/6/30)
-### v1.0.2 (2023/6/30)
-#### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
-### v1.0.1 
-#### * Fix Naming Problem
-### v1.0.0
+- v1.0.6 (2023/7/28) Fis display
+- v1.0.5 (2023/7/19) Add callback function
+- v1.0.4 (2023/7/17)
+- v1.0.3 (2023/6/30) Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
+- v1.0.1 Fix Naming Problem
+- v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues) for a list of proposed features (and known issues).
 
 ## Authors
```

### Comparing `shioaji_realtime_kbars-1.0.5/README.md` & `shioaji_realtime_kbars-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,22 +100,24 @@
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
 ### Callback funtion
+```
 shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe?
 
 Signature:
 shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe(
     contract: List[Union[shioaji.contracts.Option, shioaji.contracts.Future, shioaji.contracts.Stock, shioaji.contracts.Index]],
     last_days: int = 0,
     cb: Any = List[[callback_function, period]]
 ) -> None
+```
 
 ### Example
 If you want to clearly write your strategy. You can refer to example
 
 ```
 def strategy(period, kbars):
     print(period)
@@ -143,24 +145,20 @@
         Contracts.update(tick, "fop")
 
     Event().wait()
 ```
 
 
 ## Version
-### v1.0.5 (2023/7/19)
-#### * Add callback function
-### v1.0.4 (2023/7/17)
-#### * Fix resampling will have some NaN rows
-### v1.0.3 (2023/6/30)
-### v1.0.2 (2023/6/30)
-#### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
-### v1.0.1 
-#### * Fix Naming Problem
-### v1.0.0
+- v1.0.6 (2023/7/28) Fis display
+- v1.0.5 (2023/7/19) Add callback function
+- v1.0.4 (2023/7/17)
+- v1.0.3 (2023/6/30) Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
+- v1.0.1 Fix Naming Problem
+- v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues) for a list of proposed features (and known issues).
 
 ## Authors
```

### Comparing `shioaji_realtime_kbars-1.0.5/setup.cfg` & `shioaji_realtime_kbars-1.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_realtime_kbars
-version = 1.0.5
+version = 1.0.6
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you streaming with real-time data
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/Shioaji_Realtime_Kline
```

### Comparing `shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py` & `shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
             quote_type = sj.constant.QuoteType.Tick,
             version = sj.constant.QuoteVersion.v1
         )
 
     def update(self, tick):
         self.kbars.update({"ts" : (math.floor(int(tick.datetime.replace(tzinfo=dt.timezone.utc).timestamp() * 1000000000) / 60000000000) + 1) * 60000000000, "Open" : float(tick.open), "High" : float(tick.high), "Low" : float(tick.low), "Close" : float(tick.close), "Volume" :  tick.volume, "Amount" : float(tick.amount)})
         for cb, period in self.cb:
-            print(cb, period)
             cb(period, self.getklines(period))
 
     def getklines(self, period):
         return self.kbars.getKlines(period)
     
 class ShioajiRealtimeKbars():
```

### Comparing `shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/PKG-INFO` & `shioaji_realtime_kbars-1.0.6/src/shioaji_realtime_kbars.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji-realtime-kbars
-Version: 1.0.5
+Version: 1.0.6
 Summary: An Extensions help you streaming with real-time data
 Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -116,22 +116,24 @@
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
 ### Callback funtion
+```
 shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe?
 
 Signature:
 shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe(
     contract: List[Union[shioaji.contracts.Option, shioaji.contracts.Future, shioaji.contracts.Stock, shioaji.contracts.Index]],
     last_days: int = 0,
     cb: Any = List[[callback_function, period]]
 ) -> None
+```
 
 ### Example
 If you want to clearly write your strategy. You can refer to example
 
 ```
 def strategy(period, kbars):
     print(period)
@@ -159,24 +161,20 @@
         Contracts.update(tick, "fop")
 
     Event().wait()
 ```
 
 
 ## Version
-### v1.0.5 (2023/7/19)
-#### * Add callback function
-### v1.0.4 (2023/7/17)
-#### * Fix resampling will have some NaN rows
-### v1.0.3 (2023/6/30)
-### v1.0.2 (2023/6/30)
-#### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
-### v1.0.1 
-#### * Fix Naming Problem
-### v1.0.0
+- v1.0.6 (2023/7/28) Fis display
+- v1.0.5 (2023/7/19) Add callback function
+- v1.0.4 (2023/7/17)
+- v1.0.3 (2023/6/30) Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
+- v1.0.1 Fix Naming Problem
+- v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues) for a list of proposed features (and known issues).
 
 ## Authors
```

