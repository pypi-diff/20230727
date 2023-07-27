# Comparing `tmp/vnpy_riskmanager-1.0.3.tar.gz` & `tmp/vnpy_riskmanager-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_riskmanager-1.0.3.tar", last modified: Sun Feb 20 11:20:50 2022, max compression
+gzip compressed data, was "vnpy_riskmanager-1.0.4.tar", last modified: Thu Jul 27 08:23:22 2023, max compression
```

## Comparing `vnpy_riskmanager-1.0.3.tar` & `vnpy_riskmanager-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-02-20 11:20:49.984325 vnpy_riskmanager-1.0.3/
--rw-rw-rw-   0        0        0     1109 2021-05-23 07:34:59.000000 vnpy_riskmanager-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1930 2022-02-20 11:20:49.984325 vnpy_riskmanager-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      918 2022-02-20 11:20:09.000000 vnpy_riskmanager-1.0.3/README.md
--rw-rw-rw-   0        0        0     1037 2022-02-20 11:20:49.991685 vnpy_riskmanager-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-10-04 09:14:36.000000 vnpy_riskmanager-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-20 11:20:49.921375 vnpy_riskmanager-1.0.3/vnpy_riskmanager/
--rw-rw-rw-   0        0        0     1553 2022-02-20 11:18:37.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager/__init__.py
--rw-rw-rw-   0        0        0     8568 2022-02-20 11:18:37.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager/engine.py
-drwxrwxrwx   0        0        0        0 2022-02-20 11:20:49.982108 vnpy_riskmanager-1.0.3/vnpy_riskmanager/ui/
--rw-rw-rw-   0        0        0       33 2019-11-25 07:47:43.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager/ui/__init__.py
--rw-rw-rw-   0        0        0    59966 2019-11-25 07:47:43.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager/ui/rm.ico
--rw-rw-rw-   0        0        0     3789 2022-02-20 11:18:37.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager/ui/widget.py
-drwxrwxrwx   0        0        0        0 2022-02-20 11:20:49.974744 vnpy_riskmanager-1.0.3/vnpy_riskmanager.egg-info/
--rw-rw-rw-   0        0        0     1930 2022-02-20 11:20:49.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2022-02-20 11:20:49.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-20 11:20:49.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-20 11:20:49.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2022-02-20 11:20:49.000000 vnpy_riskmanager-1.0.3/vnpy_riskmanager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 08:23:22.120982 vnpy_riskmanager-1.0.4/
+-rw-rw-rw-   0        0        0     1109 2023-03-05 07:53:20.000000 vnpy_riskmanager-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1907 2023-07-27 08:23:22.120982 vnpy_riskmanager-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-03-05 07:53:20.000000 vnpy_riskmanager-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1037 2023-07-27 08:23:22.123026 vnpy_riskmanager-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-03-05 07:53:20.000000 vnpy_riskmanager-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:23:22.092815 vnpy_riskmanager-1.0.4/vnpy_riskmanager/
+-rw-rw-rw-   0        0        0     1627 2023-04-23 00:46:20.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager/__init__.py
+-rw-rw-rw-   0        0        0     8637 2023-04-23 00:45:39.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager/engine.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:23:22.118935 vnpy_riskmanager-1.0.4/vnpy_riskmanager/ui/
+-rw-rw-rw-   0        0        0       33 2023-03-05 07:53:20.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager/ui/__init__.py
+-rw-rw-rw-   0        0        0    59966 2023-03-05 07:53:20.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager/ui/rm.ico
+-rw-rw-rw-   0        0        0     4031 2023-07-27 08:21:56.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager/ui/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:23:22.115208 vnpy_riskmanager-1.0.4/vnpy_riskmanager.egg-info/
+-rw-rw-rw-   0        0        0     1907 2023-07-27 08:23:21.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-27 08:23:21.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:23:21.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 08:23:21.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-07-27 08:23:21.000000 vnpy_riskmanager-1.0.4/vnpy_riskmanager.egg-info/top_level.txt
```

### Comparing `vnpy_riskmanager-1.0.3/LICENSE` & `vnpy_riskmanager-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_riskmanager-1.0.3/PKG-INFO` & `vnpy_riskmanager-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy_riskmanager
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pre-trade risk management application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -52,9 +51,7 @@
 
 或者下载源代码后，解压后在cmd中运行：
 
 ```
 pip install .
 ```
 
-
-
```

### Comparing `vnpy_riskmanager-1.0.3/README.md` & `vnpy_riskmanager-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vnpy_riskmanager-1.0.3/setup.cfg` & `vnpy_riskmanager-1.0.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7269 736b 6d61 6e61   = vnpy_riskmana
 00000020: 6765 720d 0a76 6572 7369 6f6e 203d 2031  ger..version = 1
-00000030: 2e30 2e33 0d0a 7572 6c20 3d20 6874 7470  .0.3..url = http
+00000030: 2e30 2e34 0d0a 7572 6c20 3d20 6874 7470  .0.4..url = http
 00000040: 733a 2f2f 7777 772e 766e 7079 2e63 6f6d  s://www.vnpy.com
 00000050: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
 00000060: 0a61 7574 686f 7220 3d20 5869 616f 796f  .author = Xiaoyo
 00000070: 7520 4368 656e 0d0a 6175 7468 6f72 5f65  u Chen..author_e
 00000080: 6d61 696c 203d 2078 6961 6f79 6f75 2e63  mail = xiaoyou.c
 00000090: 6865 6e40 6d61 696c 2e76 6e70 792e 636f  hen@mail.vnpy.co
 000000a0: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
```

### Comparing `vnpy_riskmanager-1.0.3/vnpy_riskmanager/__init__.py` & `vnpy_riskmanager-1.0.4/vnpy_riskmanager/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from pathlib import Path
+from typing import Type
 
 from vnpy.trader.app import BaseApp
 
 from .engine import RiskEngine, APP_NAME
 
 
 class RiskManagerApp(BaseApp):
     """"""
-    app_name = APP_NAME
-    app_module = __module__
-    app_path = Path(__file__).parent
-    display_name = "交易风控"
-    engine_class = RiskEngine
-    widget_name = "RiskManager"
-    icon_name = str(app_path.joinpath("ui", "rm.ico"))
+    app_name: str = APP_NAME
+    app_module: str = __module__
+    app_path: Path = Path(__file__).parent
+    display_name: str = "交易风控"
+    engine_class: Type[RiskEngine] = RiskEngine
+    widget_name: str = "RiskManager"
+    icon_name: str = str(app_path.joinpath("ui", "rm.ico"))
```

### Comparing `vnpy_riskmanager-1.0.3/vnpy_riskmanager/engine.py` & `vnpy_riskmanager-1.0.4/vnpy_riskmanager/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-""""""
-
 from collections import defaultdict
-from typing import Callable, Dict
+from typing import Callable, Dict, Optional
 
 from vnpy.event import Event, EventEngine
 from vnpy.trader.object import OrderData, OrderRequest, LogData, TradeData
 from vnpy.trader.engine import BaseEngine, MainEngine
 from vnpy.trader.event import EVENT_TRADE, EVENT_ORDER, EVENT_LOG, EVENT_TIMER
 from vnpy.trader.constant import Direction, Status
 from vnpy.trader.utility import load_json, save_json
@@ -13,15 +11,15 @@
 
 APP_NAME = "RiskManager"
 
 
 class RiskEngine(BaseEngine):
     """风控引擎"""
 
-    setting_filename = "risk_manager_setting.json"
+    setting_filename: str = "risk_manager_setting.json"
 
     def __init__(self, main_engine: MainEngine, event_engine: EventEngine) -> None:
         """"""
         super().__init__(main_engine, event_engine, APP_NAME)
 
         self.active: bool = False
 
@@ -75,49 +73,49 @@
         if self.active:
             self.write_log("交易风控功能启动")
         else:
             self.write_log("交易风控功能停止")
 
     def get_setting(self) -> dict:
         """"""
-        setting = {
+        setting: dict = {
             "active": self.active,
             "order_flow_limit": self.order_flow_limit,
             "order_flow_clear": self.order_flow_clear,
             "order_size_limit": self.order_size_limit,
             "trade_limit": self.trade_limit,
             "active_order_limit": self.active_order_limit,
             "order_cancel_limit": self.order_cancel_limit,
         }
         return setting
 
     def load_setting(self) -> None:
         """"""
-        setting = load_json(self.setting_filename)
+        setting: dict = load_json(self.setting_filename)
         if not setting:
             return
 
         self.update_setting(setting)
 
     def save_setting(self) -> None:
         """"""
-        setting = self.get_setting()
+        setting: dict = self.get_setting()
         save_json(self.setting_filename, setting)
 
     def register_event(self) -> None:
         """"""
         self.event_engine.register(EVENT_TRADE, self.process_trade_event)
         self.event_engine.register(EVENT_TIMER, self.process_timer_event)
         self.event_engine.register(EVENT_ORDER, self.process_order_event)
 
     def process_order_event(self, event: Event) -> None:
         """"""
         order: OrderData = event.data
 
-        order_book = self.get_order_book(order.vt_symbol)
+        order_book: ActiveOrderBook = self.get_order_book(order.vt_symbol)
         order_book.update_order(order)
 
         if order.status != Status.CANCELLED:
             return
         self.order_cancel_counts[order.vt_symbol] += 1
 
     def process_trade_event(self, event: Event) -> None:
@@ -170,39 +168,39 @@
         active_order_count: int = len(self.main_engine.get_all_active_orders())
         if active_order_count >= self.active_order_limit:
             self.write_log(
                 f"当前活动委托次数{active_order_count}，超过限制{self.active_order_limit}")
             return False
 
         # Check order cancel counts
-        order_cancel_count = self.order_cancel_counts.get(req.vt_symbol, 0)
+        order_cancel_count: int = self.order_cancel_counts.get(req.vt_symbol, 0)
         if order_cancel_count >= self.order_cancel_limit:
             self.write_log(f"当日{req.vt_symbol}撤单次数{order_cancel_count}，超过限制{self.order_cancel_limit}")
             return False
 
         # Check order self trade
         order_book: ActiveOrderBook = self.get_order_book(req.vt_symbol)
         if req.direction == Direction.LONG:
-            best_ask = order_book.get_best_ask()
+            best_ask: float = order_book.get_best_ask()
             if best_ask and req.price >= best_ask:
                 self.write_log(f"买入价格{req.price}大于等于已挂最低卖价{best_ask}，可能导致自成交")
                 return False
         else:
-            best_bid = order_book.get_best_bid()
+            best_bid: float = order_book.get_best_bid()
             if best_bid and req.price <= best_bid:
                 self.write_log(f"卖出价格{req.price}小于等于已挂最低买价{best_bid}，可能导致自成交")
                 return False
 
         # Add flow count if pass all checks
         self.order_flow_count += 1
         return True
 
     def get_order_book(self, vt_symbol: str) -> "ActiveOrderBook":
         """"""
-        order_book: ActiveOrderBook = self.active_order_books.get(vt_symbol, None)
+        order_book: Optional[ActiveOrderBook] = self.active_order_books.get(vt_symbol, None)
         if not order_book:
             order_book = ActiveOrderBook(vt_symbol)
             self.active_order_books[vt_symbol] = order_book
         return order_book
 
 
 class ActiveOrderBook:
```

### Comparing `vnpy_riskmanager-1.0.3/vnpy_riskmanager/ui/rm.ico` & `vnpy_riskmanager-1.0.4/vnpy_riskmanager/ui/rm.ico`

 * *Files identical despite different names*

### Comparing `vnpy_riskmanager-1.0.3/vnpy_riskmanager/ui/widget.py` & `vnpy_riskmanager-1.0.4/vnpy_riskmanager/ui/widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from vnpy.event import EventEngine
 from vnpy.trader.engine import MainEngine
-from vnpy.trader.ui import QtWidgets
+from vnpy.trader.ui import QtWidgets, QtCore
 
 from ..engine import APP_NAME, RiskEngine
 
 
 class RiskManager(QtWidgets.QDialog):
     """"""
 
@@ -19,53 +19,53 @@
         self.init_ui()
 
     def init_ui(self) -> None:
         """"""
         self.setWindowTitle("交易风控")
 
         # Create widgets
-        self.active_combo = QtWidgets.QComboBox()
+        self.active_combo: QtWidgets.QComboBox = QtWidgets.QComboBox()
         self.active_combo.addItems(["停止", "启动"])
 
-        self.flow_limit_spin = RiskManagerSpinBox()
-        self.flow_clear_spin = RiskManagerSpinBox()
-        self.size_limit_spin = RiskManagerSpinBox()
-        self.trade_limit_spin = RiskManagerSpinBox()
-        self.active_limit_spin = RiskManagerSpinBox()
-        self.cancel_limit_spin = RiskManagerSpinBox()
+        self.flow_limit_spin: RiskManagerSpinBox = RiskManagerSpinBox()
+        self.flow_clear_spin: RiskManagerSpinBox = RiskManagerSpinBox()
+        self.size_limit_spin: RiskManagerSpinBox = RiskManagerSpinBox()
+        self.trade_limit_spin: RiskManagerSpinBox = RiskManagerSpinBox()
+        self.active_limit_spin: RiskManagerSpinBox = RiskManagerSpinBox()
+        self.cancel_limit_spin: RiskManagerSpinBox = RiskManagerSpinBox()
 
-        save_button = QtWidgets.QPushButton("保存")
+        save_button: QtWidgets.QPushButton = QtWidgets.QPushButton("保存")
         save_button.clicked.connect(self.save_setting)
 
         # Form layout
-        form = QtWidgets.QFormLayout()
+        form: QtWidgets.QFormLayout = QtWidgets.QFormLayout()
         form.addRow("风控运行状态", self.active_combo)
         form.addRow("委托流控上限（笔）", self.flow_limit_spin)
         form.addRow("委托流控清空（秒）", self.flow_clear_spin)
         form.addRow("单笔委托上限（数量）", self.size_limit_spin)
         form.addRow("总成交上限（笔）", self.trade_limit_spin)
         form.addRow("活动委托上限（笔）", self.active_limit_spin)
         form.addRow("合约撤单上限（笔）", self.cancel_limit_spin)
         form.addRow(save_button)
 
         self.setLayout(form)
 
         # Set Fix Size
-        hint = self.sizeHint()
+        hint: QtCore.QSize = self.sizeHint()
         self.setFixedSize(int(hint.width() * 1.2), hint.height())
 
     def save_setting(self) -> None:
         """"""
-        active_text = self.active_combo.currentText()
+        active_text: str = self.active_combo.currentText()
         if active_text == "启动":
-            active = True
+            active: bool = True
         else:
-            active = False
+            active: bool = False
 
-        setting = {
+        setting: dict = {
             "active": active,
             "order_flow_limit": self.flow_limit_spin.value(),
             "order_flow_clear": self.flow_clear_spin.value(),
             "order_size_limit": self.size_limit_spin.value(),
             "trade_limit": self.trade_limit_spin.value(),
             "active_order_limit": self.active_limit_spin.value(),
             "order_cancel_limit": self.cancel_limit_spin.value(),
@@ -74,36 +74,36 @@
         self.rm_engine.update_setting(setting)
         self.rm_engine.save_setting()
 
         self.close()
 
     def update_setting(self) -> None:
         """"""
-        setting = self.rm_engine.get_setting()
+        setting: dict = self.rm_engine.get_setting()
         if setting["active"]:
             self.active_combo.setCurrentIndex(1)
         else:
             self.active_combo.setCurrentIndex(0)
 
         self.flow_limit_spin.setValue(setting["order_flow_limit"])
         self.flow_clear_spin.setValue(setting["order_flow_clear"])
         self.size_limit_spin.setValue(setting["order_size_limit"])
         self.trade_limit_spin.setValue(setting["trade_limit"])
         self.active_limit_spin.setValue(setting["active_order_limit"])
         self.cancel_limit_spin.setValue(setting["order_cancel_limit"])
 
-    def exec_(self) -> None:
+    def exec(self) -> None:
         """"""
         self.update_setting()
-        super().exec_()
+        super().exec()
 
 
 class RiskManagerSpinBox(QtWidgets.QSpinBox):
     """"""
 
     def __init__(self, value: int = 0) -> None:
         """"""
         super().__init__()
 
         self.setMinimum(0)
-        self.setMaximum(1000000)
+        self.setMaximum(1_000_000_000)
         self.setValue(value)
```

### Comparing `vnpy_riskmanager-1.0.3/vnpy_riskmanager.egg-info/PKG-INFO` & `vnpy_riskmanager-1.0.4/vnpy_riskmanager.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vnpy-riskmanager
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pre-trade risk management application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -52,9 +51,7 @@
 
 或者下载源代码后，解压后在cmd中运行：
 
 ```
 pip install .
 ```
 
-
-
```

