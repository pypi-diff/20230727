# Comparing `tmp/vnpy_icetcore-1.0.0-py3-none-any.whl.zip` & `tmp/vnpy_icetcore-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12013 bytes, number of entries: 10
+Zip file size: 11195 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      365 b- defN 23-Jul-27 07:41 vnpy_icetcore/__init__.py
--rw-rw-rw-  2.0 fat    10882 b- defN 23-Jul-27 05:11 vnpy_icetcore/icetcore_datafeed.py
--rw-rw-rw-  2.0 fat    27991 b- defN 23-Jul-27 07:58 vnpy_icetcore/icetcore_gateway.py
+-rw-rw-rw-  2.0 fat     8219 b- defN 23-Jul-27 09:14 vnpy_icetcore/icetcore_datafeed.py
+-rw-rw-rw-  2.0 fat    27831 b- defN 23-Jul-27 09:14 vnpy_icetcore/icetcore_gateway.py
 -rw-rw-rw-  2.0 fat        1 b- defN 22-Dec-16 01:53 vnpy_icetcore/sample/__init__.py
 -rw-rw-rw-  2.0 fat     1898 b- defN 23-Jul-27 07:15 vnpy_icetcore/sample/run.py
--rw-rw-rw-  2.0 fat       30 b- defN 23-Jul-27 08:01 vnpy_icetcore-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      359 b- defN 23-Jul-27 08:01 vnpy_icetcore-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 08:01 vnpy_icetcore-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-27 08:01 vnpy_icetcore-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      847 b- defN 23-Jul-27 08:01 vnpy_icetcore-1.0.0.dist-info/RECORD
-10 files, 42479 bytes uncompressed, 10551 bytes compressed:  75.2%
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Jul-27 09:16 vnpy_icetcore-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      359 b- defN 23-Jul-27 09:16 vnpy_icetcore-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 09:16 vnpy_icetcore-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-27 09:16 vnpy_icetcore-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      846 b- defN 23-Jul-27 09:16 vnpy_icetcore-1.0.1.dist-info/RECORD
+10 files, 39655 bytes uncompressed, 9733 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: vnpy_icetcore/sample/__init__.py
 Comment: 
 
 Filename: vnpy_icetcore/sample/run.py
 Comment: 
 
-Filename: vnpy_icetcore-1.0.0.dist-info/LICENSE
+Filename: vnpy_icetcore-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: vnpy_icetcore-1.0.0.dist-info/METADATA
+Filename: vnpy_icetcore-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: vnpy_icetcore-1.0.0.dist-info/WHEEL
+Filename: vnpy_icetcore-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: vnpy_icetcore-1.0.0.dist-info/top_level.txt
+Filename: vnpy_icetcore-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vnpy_icetcore-1.0.0.dist-info/RECORD
+Filename: vnpy_icetcore-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vnpy_icetcore/icetcore_datafeed.py

```diff
@@ -38,121 +38,35 @@
     Interval.DAILY: timedelta()         # no need to adjust for daily bar
 }
 
 
 
 CHINA_TZ = ZoneInfo("Asia/Shanghai")
 
-
-def to_rq_symbol(symbol: str, exchange: Exchange, all_symbols: ndarray) -> str:
-    """将交易所代码转换为米筐代码"""
-    # 股票
-    if exchange in {Exchange.SSE, Exchange.SZSE}:
-        if exchange == Exchange.SSE:
-            rq_symbol: str = f"{symbol}.XSHG"
-        else:
-            rq_symbol: str = f"{symbol}.XSHE"
-    # 金交所现货
-    elif exchange == Exchange.SGE:
-        for char in ["(", ")", "+"]:
-            symbol: str = symbol.replace(char, "")
-        symbol = symbol.upper()
-        rq_symbol: str = f"{symbol}.SGEX"
-    # 期货和期权
-    elif exchange in {
-        Exchange.CFFEX,
-        Exchange.SHFE,
-        Exchange.DCE,
-        Exchange.CZCE,
-        Exchange.INE,
-        Exchange.GFEX
-    }:
-        for count, word in enumerate(symbol):
-            if word.isdigit():
-                break
-
-        product: str = symbol[:count]
-        time_str: str = symbol[count:]
-
-        # 期货
-        if time_str.isdigit():
-            # 只有郑商所需要特殊处理
-            if exchange is not Exchange.CZCE:
-                return symbol.upper()
-
-            # 检查是否为连续合约或者指数合约
-            if time_str in ["88", "888", "99", "889"]:
-                return symbol
-
-            # 提取年月
-            year: str = symbol[count]
-            month: str = symbol[count + 1:]
-
-            guess_1: str = f"{product}1{year}{month}".upper()
-            guess_2: str = f"{product}2{year}{month}".upper()
-
-            # 优先尝试20年后的合约
-            if guess_2 in all_symbols:
-                rq_symbol: str = guess_2
-            else:
-                rq_symbol: str = guess_1
-        # 期权
-        else:
-            if exchange in {
-                Exchange.CFFEX,
-                Exchange.DCE,
-                Exchange.SHFE,
-                Exchange.INE,
-                Exchange.GFEX
-            }:
-                rq_symbol: str = symbol.replace("-", "").upper()
-            elif exchange == Exchange.CZCE:
-                year: str = symbol[count]
-                suffix: str = symbol[count + 1:]
-
-                guess_1: str = f"{product}1{year}{suffix}".upper()
-                guess_2: str = f"{product}2{year}{suffix}".upper()
-
-                # 优先尝试20年后的合约
-                if guess_2 in all_symbols:
-                    rq_symbol: str = guess_2
-                else:
-                    rq_symbol: str = guess_1
-    else:
-        rq_symbol: str = f"{symbol}.{exchange.value}"
-
-    return rq_symbol
-
-
-
 class IceTCoreDatafeed(BaseDatafeed):
     """
     VeighNa用于对接期货CTP柜台的交易接口。
     """
     default_name: str = "ICETCore"
-    default_setting: Dict[str, str] = {
-        "产品名称": "",
-        "授权编码": ""
-    }
+
 
     exchanges: List[str] = list(EXCHANGE_ICE2VT.values())
 
     def __init__(self):
         """"""
         self.username: str = SETTINGS["datafeed.username"]
-        self.password: str = SETTINGS["datafeed.password"]
         self.api: "TCoreAPI" =TCoreAPI()
         self.inited: bool = False
         self.symbols: ndarray = None
 
     def init(self, output: Callable = print) -> bool:
         """初始化"""
         if self.inited:
             return True
-        self.api.connect()
+        self.api.connect(appid=self.username)
         self.inited = True
         return True
 
 
     def write_error(self, msg: str, error: dict) -> None:
         """输出错误信息日志"""
         error_id: int = error["ErrorID"]
```

## vnpy_icetcore/icetcore_gateway.py

```diff
@@ -188,16 +188,15 @@
 
 class IceTCoreGateway(BaseGateway,BaseDatafeed):
     """
     VeighNa用于对接期货CTP柜台的交易接口。
     """
     default_name: str = "ICETCore"
     default_setting: Dict[str, str] = {
-        "产品名称": "",
-        "授权编码": ""
+        "产品名称": ""
     }
 
     exchanges: List[str] = list(EXCHANGE_ICE2VT.values())
 
     def __init__(self, event_engine: EventEngine, gateway_name: str) -> None:
         """构造函数"""
         super().__init__(event_engine, gateway_name)
@@ -219,20 +218,19 @@
         self.userid: str = ""
         self.brokerid: str = ""
         self.auth_code: str = ""
         self.appid: str = ""
 
     def connect(self, setting: dict) -> None:
         """连接交易接口"""
-        appid: str = setting["产品名称"]
-        auth_code: str = setting["授权编码"]
+        self.appid: str = setting["产品名称"]
 
         # 禁止重复发起连接，会导致异常崩溃
         if not self.connect_status:
-            self.api.connect(appid="AlgoMaster2DEV",servicekey="8076c9867a372d2a9a814ae710c256e2")#(self.appid,self.auth_code)
+            self.api.connect(appid=self.appid)#(self.appid,self.auth_code)
             self.connect_status = True
             self.qryInstrument()
         #self.init_query()
 
     def subscribe(self, req: SubscribeRequest) -> None:
         """订阅行情"""
         self.write_log("订阅行情"+req.symbol)
@@ -469,15 +467,14 @@
     def __init__(self, gateway: IceTCoreGateway) -> None:
         """构造函数"""
         self.subscribed: set = set()
         self.gateway: IceTCoreGateway = gateway
         self.gateway_name: str = gateway.gateway_name
 
         self.sysid_orderid_map: Dict[str, str] = {}
-
         self.current_date: str = datetime.now().strftime("%Y%m%d")
 
     def onconnected(self,apitype:str) -> None:
         """服务器连接成功回报"""
         if "quote"==apitype:
             self.login_status = True
             self.gateway.write_log("行情接口连线成功")
@@ -607,15 +604,14 @@
         self.sysid_orderid_map[data["UserKey1"]] = data["ReportID"]
 
 
     def onfilledreportreal(self,data):
         """成交数据推送"""
         if not self.gateway.contract_inited:
             return
-        print("成交回报",data)
         symbsplit=data["Symbol"].split(".")
         symbol: str = data["Symbol"].replace(symbsplit[0]+"."+symbsplit[1]+"."+symbsplit[2]+".","").replace(".","")
         contract: ContractData = symbol_contract_map.get(symbsplit[2]+"."+symbol, None)
 
         orderid: str = self.sysid_orderid_map[data["UserKey1"]]
 
         timestamp: str = f"{data['TransactDate']} {data['TransactTime']}"
```

## Comparing `vnpy_icetcore-1.0.0.dist-info/RECORD` & `vnpy_icetcore-1.0.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 vnpy_icetcore/__init__.py,sha256=vlksCqG8ci0F3UyKOvMiU7XJUadwlO0as1rDo7Ri1Nc,365
-vnpy_icetcore/icetcore_datafeed.py,sha256=7DTjBKAUnNCAWn1p9TySVWBlunmYbwfw8c_a91sPNwo,10882
-vnpy_icetcore/icetcore_gateway.py,sha256=CRUU3QT8NqVC_pIpSjIVw_Y_APaDqQPO9Xlg7xUtvjo,27991
+vnpy_icetcore/icetcore_datafeed.py,sha256=6ISl7HaOQP_bH7Owt1uCfYs_09TulSIVfXduEtmt41I,8219
+vnpy_icetcore/icetcore_gateway.py,sha256=_40TdbngD07BiARaRwT2ne5NqvPNAFyiWySsTgGyz0U,27831
 vnpy_icetcore/sample/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 vnpy_icetcore/sample/run.py,sha256=HmiKYJKhEyFbMWkM33a48Nxc7aUQkeawIjSCepciLf4,1898
-vnpy_icetcore-1.0.0.dist-info/LICENSE,sha256=mQl03LAdwPIUbhG7swmKCJxrLH4XbG_nLJ6vthUG1ZY,30
-vnpy_icetcore-1.0.0.dist-info/METADATA,sha256=lF-m3HdQweZcm-6oOnVTqdXsg_A8ZlhFFqMbu6-rPqI,359
-vnpy_icetcore-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vnpy_icetcore-1.0.0.dist-info/top_level.txt,sha256=aWQFbP-ECltOd0qINgHp1615sTYi_Zxc8X0ITb_7ttc,14
-vnpy_icetcore-1.0.0.dist-info/RECORD,,
+vnpy_icetcore-1.0.1.dist-info/LICENSE,sha256=mQl03LAdwPIUbhG7swmKCJxrLH4XbG_nLJ6vthUG1ZY,30
+vnpy_icetcore-1.0.1.dist-info/METADATA,sha256=FUTPgaqqQF1YI5BKhQk5KlgDSDXqO8qu6eLsHuWC0Cg,359
+vnpy_icetcore-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vnpy_icetcore-1.0.1.dist-info/top_level.txt,sha256=aWQFbP-ECltOd0qINgHp1615sTYi_Zxc8X0ITb_7ttc,14
+vnpy_icetcore-1.0.1.dist-info/RECORD,,
```

