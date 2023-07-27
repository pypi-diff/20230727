# Comparing `tmp/xtb_broker-0.0.7.tar.gz` & `tmp/xtb_broker-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtb_broker-0.0.7.tar", last modified: Fri Jul 21 09:26:48 2023, max compression
+gzip compressed data, was "xtb_broker-0.0.8.tar", last modified: Thu Jul 27 17:01:32 2023, max compression
```

## Comparing `xtb_broker-0.0.7.tar` & `xtb_broker-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      453 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/README.md
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:52:23.000000 xtb_broker-0.0.7/pyproject.toml
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/setup.cfg
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      397 2023-07-21 09:26:43.000000 xtb_broker-0.0.7/setup.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.825466 xtb_broker-0.0.7/xtb_broker/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12091 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/client.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.825466 xtb_broker-0.0.7/xtb_broker/config/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/config/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.7/xtb_broker/config/constants.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/config/exception.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      697 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/config/frozen.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      285 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/config/logger.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/xtb_broker/models/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/models/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     5996 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/arbitrage.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2178 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/position.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      579 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/models/shift.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3075 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/symbol.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/timetable.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6445 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/trade.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/models/transaction.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/utils.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2639 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/xtb.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.825466 xtb_broker-0.0.7/xtb_broker.egg-info/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      636 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/top_level.txt
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      453 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/README.md
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:52:23.000000 xtb_broker-0.0.8/pyproject.toml
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/setup.cfg
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      397 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/setup.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12091 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/client.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker/config/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/config/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.8/xtb_broker/config/constants.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/config/exception.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      697 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/config/frozen.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      285 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/config/logger.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker/models/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/models/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     5996 2023-07-21 09:26:28.000000 xtb_broker-0.0.8/xtb_broker/models/arbitrage.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2178 2023-07-21 09:26:28.000000 xtb_broker-0.0.8/xtb_broker/models/position.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      579 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/models/shift.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2638 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/xtb_broker/models/symbol.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1247 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/xtb_broker/models/tick.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:28.000000 xtb_broker-0.0.8/xtb_broker/models/timetable.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6479 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/xtb_broker/models/trade.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/models/transaction.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/utils.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2535 2023-07-22 11:42:12.000000 xtb_broker-0.0.8/xtb_broker/xtb.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker.egg-info/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      662 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/top_level.txt
```

### Comparing `xtb_broker-0.0.7/pyproject.toml` & `xtb_broker-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/client.py` & `xtb_broker-0.0.8/xtb_broker/client.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/config/constants.py` & `xtb_broker-0.0.8/xtb_broker/config/constants.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/config/exception.py` & `xtb_broker-0.0.8/xtb_broker/config/exception.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/config/frozen.py` & `xtb_broker-0.0.8/xtb_broker/config/frozen.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/models/arbitrage.py` & `xtb_broker-0.0.8/xtb_broker/models/arbitrage.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/models/position.py` & `xtb_broker-0.0.8/xtb_broker/models/position.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/models/shift.py` & `xtb_broker-0.0.8/xtb_broker/models/shift.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/models/symbol.py` & `xtb_broker-0.0.8/xtb_broker/models/symbol.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,111 +5,92 @@
 from config.constants import WEEKDAY
 from models.timetable import Timetable
 from models.shift import Shift
 
 from xtb import Xtb
 
 
-
 class Symbol(Frozen):
     def __init__(self, xtb: Xtb, symbol: str):
         symbol_dict: Dict = xtb.get_client().get_symbol(symbol=symbol)
         self.__symbol: str = symbol_dict['symbol']
         self.__currency: str = symbol_dict['currency']
         self.__currency_profit: str = symbol_dict['currencyProfit']
         self.__contract_size: str = symbol_dict['contractSize']
         self.__precision: str = symbol_dict['precision']
         self.__bid: str = symbol_dict['bid']
         self.__ask: str = symbol_dict['ask']
         self.__swap_long: str = symbol_dict['swapLong']
         self.__swap_short: str = symbol_dict['swapShort']
         self.__spread: float = symbol_dict['spreadRaw']
+
+        self.__time: int = symbol_dict['time']
+        self.__pips_precision: int = symbol_dict['pipsPrecision']
+        self.__tick_size: float = symbol_dict['tickSize']
+        self.__leverage: float = symbol_dict['leverage']
+
         self.__timetable: Timetable = xtb.get_symbol_timetable(symbol=symbol)
-        
+
     @property
     def symbol(self) -> str:
         return self.__symbol
 
-    @symbol.setter
-    def symbol(self, value: str) -> None:
-        self.__symbol = value
-
     @property
     def currency(self) -> str:
         return self.__currency
 
-    @currency.setter
-    def currency(self, value: str) -> None:
-        self.__currency = value
-
     @property
     def currency_profit(self) -> str:
         return self.__currency_profit
 
     @property
     def contract_size(self) -> str:
         return self.__contract_size
 
-    @contract_size.setter
-    def contract_size(self, value: str) -> None:
-        self.__contract_size = value
-
     @property
     def precision(self) -> str:
         return self.__precision
 
-    @precision.setter
-    def precision(self, value: str) -> None:
-        self.__precision = value
-
     @property
     def bid(self) -> str:
         return self.__bid
 
-    @bid.setter
-    def bid(self, value: str) -> None:
-        self.__bid = value
-
     @property
     def ask(self) -> str:
         return self.__ask
 
-    @ask.setter
-    def ask(self, value: str) -> None:
-        self.__ask = value
-
     @property
     def swap_long(self) -> str:
         return self.__swap_long
 
-    @swap_long.setter
-    def swap_long(self, value: str) -> None:
-        self.__swap_long = value
-
     @property
     def swap_short(self) -> str:
         return self.__swap_short
 
-    @swap_short.setter
-    def swap_short(self, value: str) -> None:
-        self.__swap_short = value
-
     @property
     def timetable(self) -> Timetable:
         return self.__timetable
 
-    @timetable.setter
-    def timetable(self, value: Timetable) -> None:
-        self.__timetable = value
-
     @property
     def spread(self) -> float:
         return self.__spread
 
-    @spread.setter
-    def spread(self, value: float) -> None:
-        self.__spread = value
+    @property
+    def time(self) -> int:
+        return self.__time
+
+    @property
+    def pips_precision(self) -> int:
+        return self.__pips_precision
+
+    @property
+    def tick_size(self) -> float:
+        return self.__tick_size
+
+    @property
+    def leverage(self) -> float:
+        return self.__leverage
 
     def get_active_shift(self) -> Optional[Shift]:
         for shift in getattr(self.timetable, WEEKDAY[datetime.today().isoweekday()]):
             if shift.from_ts < datetime.now() < shift.to_ts:
                 return shift
```

### Comparing `xtb_broker-0.0.7/xtb_broker/models/timetable.py` & `xtb_broker-0.0.8/xtb_broker/models/timetable.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/models/transaction.py` & `xtb_broker-0.0.8/xtb_broker/models/transaction.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/utils.py` & `xtb_broker-0.0.8/xtb_broker/utils.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.7/xtb_broker/xtb.py` & `xtb_broker-0.0.8/xtb_broker/xtb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from typing import Optional, Dict
 from retrying import retry
 from datetime import datetime
-import sys
-import os
-
-sys.path.append(os.path.realpath(os.path.join(os.path.dirname(__file__), '.')))
 from config.constants import WEEKDAY
 from models.timetable import Timetable
 from models.shift import Shift
 from utils import ts_to_unix_ts
 import client
 from client import XtbClient
 
 
-
 # Declared at cold-start, but only initialized if/when the function executes (initializing them lazily on demand)
 xtb_client: Optional[XtbClient] = None
 
 
 class Xtb:
     def __init__(self, mode: str):
         self.__mode: str = mode
@@ -64,8 +59,7 @@
     def get_trade_record(self, order: int) -> Dict:
         return self.get_client().get_trade_records(orders=[order])[0]
 
 
 @retry(stop_max_attempt_number=3, wait_random_min=1000, wait_random_max=2000)
 def get_xtb_client(mode: str) -> XtbClient:
     return XtbClient(mode)
-
```

### Comparing `xtb_broker-0.0.7/xtb_broker.egg-info/SOURCES.txt` & `xtb_broker-0.0.8/xtb_broker.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 xtb_broker/config/frozen.py
 xtb_broker/config/logger.py
 xtb_broker/models/__init__.py
 xtb_broker/models/arbitrage.py
 xtb_broker/models/position.py
 xtb_broker/models/shift.py
 xtb_broker/models/symbol.py
+xtb_broker/models/tick.py
 xtb_broker/models/timetable.py
 xtb_broker/models/trade.py
 xtb_broker/models/transaction.py
```

