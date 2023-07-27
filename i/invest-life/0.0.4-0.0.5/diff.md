# Comparing `tmp/invest_life-0.0.4.tar.gz` & `tmp/invest_life-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_life-0.0.4.tar", last modified: Thu Jul 27 08:39:05 2023, max compression
+gzip compressed data, was "invest_life-0.0.5.tar", last modified: Thu Jul 27 09:30:39 2023, max compression
```

## Comparing `invest_life-0.0.4.tar` & `invest_life-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.073386 invest_life-0.0.4/
--rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.4/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 08:39:05.070343 invest_life-0.0.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.4/README.md
--rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-27 08:38:55.000000 invest_life-0.0.4/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-27 08:39:05.074706 invest_life-0.0.4/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.061653 invest_life-0.0.4/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.4/src/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.067603 invest_life-0.0.4/src/invest_life.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)   212847 2023-07-27 08:37:55.000000 invest_life-0.0.4/src/investlife.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.069466 invest_life-0.0.4/tests/
--rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.4/tests/test.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.291898 invest_life-0.0.5/
+-rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.5/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 09:30:39.291588 invest_life-0.0.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.5/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-27 09:30:21.000000 invest_life-0.0.5/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-27 09:30:39.291995 invest_life-0.0.5/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.288093 invest_life-0.0.5/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.5/src/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.290208 invest_life-0.0.5/src/invest_life.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-27 09:30:39.000000 invest_life-0.0.5/src/invest_life.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)   221418 2023-07-27 09:30:14.000000 invest_life-0.0.5/src/investlife.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 09:30:39.290622 invest_life-0.0.5/tests/
+-rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.5/tests/test.py
```

### Comparing `invest_life-0.0.4/LICENSE` & `invest_life-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `invest_life-0.0.4/PKG-INFO` & `invest_life-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_life
-Version: 0.0.4
+Version: 0.0.5
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.4/src/invest_life.egg-info/PKG-INFO` & `invest_life-0.0.5/src/invest_life.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-life
-Version: 0.0.4
+Version: 0.0.5
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.4/src/investlife.py` & `invest_life-0.0.5/src/investlife.py`

 * *Files 2% similar despite different names*

```diff
@@ -804,14 +804,121 @@
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
         return pickle.loads(res.content)
 
     return res.text
 
+def get_stock_quote_realtime():
+    """
+    获取单个或者多个市场行情的最新状况
+
+    Parameters
+    ----------
+    fs : Union[str, List[str]], optional
+        行情名称或者多个行情名列表 可选值及示例如下
+
+        - ``None``  沪深京A股市场行情
+        - ``'沪深A股'`` 沪深A股市场行情
+        - ``'沪A'`` 沪市A股市场行情
+        - ``'深A'`` 深市A股市场行情
+        - ``北A``   北证A股市场行情
+        - ``'可转债'``  沪深可转债市场行情
+        - ``'期货'``    期货市场行情
+        - ``'创业板'``  创业板市场行情
+        - ``'美股'``    美股市场行情
+        - ``'港股'``    港股市场行情
+        - ``'中概股'``  中国概念股市场行情
+        - ``'新股'``    沪深新股市场行情
+        - ``'科创板'``  科创板市场行情
+        - ``'沪股通'``  沪股通市场行情
+        - ``'深股通'``  深股通市场行情
+        - ``'行业板块'``    行业板块市场行情
+        - ``'概念板块'``    概念板块市场行情
+        - ``'沪深系列指数'``    沪深系列指数市场行情
+        - ``'上证系列指数'``    上证系列指数市场行情
+        - ``'深证系列指数'``    深证系列指数市场行情
+        - ``'ETF'`` ETF 基金市场行情
+        - ``'LOF'`` LOF 基金市场行情
+
+
+    Returns
+    -------
+    DataFrame
+        单个或者多个市场行情的最新状况
+
+    Raises
+    ------
+    KeyError
+        当参数 ``fs`` 中含有不正确的行情类型时引发错误
+
+    Examples
+    --------
+    >>> import efinance as ef
+    >>> ef.stock.get_realtime_quotes()
+            股票代码   股票名称     涨跌幅     最新价      最高      最低      今开     涨跌额    换手率    量比    动态市盈率     成交量           成交额   昨日收盘           总市值         流通市值      行情ID 市场类型
+    0     688787    N海天  277.59  139.48  172.39  139.25  171.66  102.54  85.62     -    78.93   74519  1110318832.0  36.94    5969744000   1213908667  1.688787   沪A
+    1     301045    N天禄  149.34   39.42   48.95    39.2   48.95   23.61  66.66     -    37.81  163061   683878656.0  15.81    4066344240    964237089  0.301045   深A
+    2     300532   今天国际   20.04   12.16   12.16   10.69   10.69    2.03   8.85  3.02   -22.72  144795   171535181.0  10.13    3322510580   1989333440  0.300532   深A
+    3     300600   国瑞科技   20.02   13.19   13.19   11.11   11.41     2.2  18.61  2.82   218.75  423779   541164432.0  10.99    3915421427   3003665117  0.300600   深A
+    4     300985   致远新能   20.01   47.08   47.08    36.8    39.4    7.85  66.65  2.17    58.37  210697   897370992.0  39.23    6277336472   1488300116  0.300985   深A
+    ...      ...    ...     ...     ...     ...     ...     ...     ...    ...   ...      ...     ...           ...    ...           ...          ...       ...  ...
+    4598  603186   华正新材   -10.0   43.27   44.09   43.27   43.99   -4.81   1.98  0.48    25.24   27697   120486294.0  48.08    6146300650   6063519472  1.603186   沪A
+    4599  688185  康希诺-U  -10.11   476.4  534.94  460.13   530.0   -53.6   6.02  2.74 -2088.07   40239  1960540832.0  530.0  117885131884  31831479215  1.688185   沪A
+    4600  688148   芳源股份  -10.57    31.3   34.39    31.3    33.9    -3.7  26.07  0.56   220.01  188415   620632512.0   35.0   15923562000   2261706043  1.688148   沪A
+    4601  300034   钢研高纳  -10.96   43.12   46.81   42.88    46.5   -5.31   7.45  1.77    59.49  323226  1441101824.0  48.43   20959281094  18706911861  0.300034   深A
+    4602  300712   永福股份  -13.71    96.9  110.94    95.4   109.0   -15.4   6.96  1.26   511.21  126705  1265152928.0  112.3   17645877600  17645877600  0.300712   深A
+
+    >>> ef.stock.get_realtime_quotes(['创业板','港股'])
+        股票代码    股票名称    涨跌幅    最新价     最高     最低     今开    涨跌额   换手率     量比   动态市盈率       成交量         成交额   昨日收盘         总市值        流通市值       行情ID  市场类型
+    0     00859  中昌国际控股  49.02   0.38   0.38   0.26   0.26  0.125  0.08  86.85   -2.83    938000    262860.0  0.255   427510287   427510287  128.00859  None
+    1     01058    粤海制革  41.05   1.34   1.51    0.9   0.93   0.39  8.34   1.61  249.89  44878000  57662440.0   0.95   720945460   720945460  128.01058  None
+    2     00713  世界(集团)  27.94   0.87    0.9   0.68   0.68   0.19  1.22  33.28    3.64   9372000   7585400.0   0.68   670785156   670785156  128.00713  None
+    3     08668    瀛海集团  24.65  0.177  0.179  0.145  0.145  0.035   0.0   10.0   -9.78     20000      3240.0  0.142   212400000   212400000  128.08668  None
+    4     08413    亚洲杂货  24.44   0.28   0.28   0.25   0.25  0.055  0.01   3.48  -20.76    160000     41300.0  0.225   325360000   325360000  128.08413  None
+    ...     ...     ...    ...    ...    ...    ...    ...    ...   ...    ...     ...       ...         ...    ...         ...         ...        ...   ...
+    5632  08429    冰雪集团 -16.75  0.174    0.2  0.166    0.2 -0.035  2.48   3.52  -21.58  11895000   2074645.0  0.209    83520000    83520000  128.08429  None
+    5633  00524    长城天下 -17.56  0.108  0.118  0.103  0.118 -0.023  0.45  15.43   -6.55   5961200    649171.0  0.131   141787800   141787800  128.00524  None
+    5634  08377    申酉控股 -17.71  0.395   0.46   0.39   0.46 -0.085  0.07   8.06   -5.07    290000    123200.0   0.48   161611035   161611035  128.08377  None
+    5635  00108    国锐地产 -19.01   1.15   1.42   1.15   1.42  -0.27  0.07   0.78   23.94   2376000   3012080.0   1.42  3679280084  3679280084  128.00108  None
+    5636  08237    华星控股  -25.0  0.024  0.031  0.023  0.031 -0.008  0.43   8.74   -2.01  15008000    364188.0  0.032    83760000    83760000  128.08237  None
+
+    >>> ef.stock.get_realtime_quotes(['ETF'])
+        股票代码         股票名称   涨跌幅    最新价     最高     最低     今开    涨跌额    换手率    量比 动态市盈率       成交量           成交额   昨日收盘          总市值         流通市值      行情ID 市场类型
+    0    513050     中概互联网ETF  4.49  1.444  1.455  1.433  1.452  0.062   6.71  0.92     -  12961671  1870845984.0  1.382  27895816917  27895816917  1.513050   沪A
+    1    513360        教育ETF  4.38    0.5  0.502  0.486  0.487  0.021  16.89   1.7     -   1104254    54634387.0  0.479    326856952    326856952  1.513360   沪A
+    2    159766        旅游ETF  3.84  0.974  0.988   0.95   0.95  0.036  14.46  1.97     -    463730    45254947.0  0.938    312304295    312304295  0.159766   深A
+    3    159865        养殖ETF   3.8  0.819  0.828  0.785  0.791   0.03  12.13  0.89     -   1405871   114254714.0  0.789    949594189    949594189  0.159865   深A
+    4    516670      畜牧养殖ETF  3.76  0.856  0.864  0.825  0.835  0.031  24.08  0.98     -    292027    24924513.0  0.825    103803953    103803953  1.516670   沪A
+    ..      ...          ...   ...    ...    ...    ...    ...    ...    ...   ...   ...       ...           ...    ...          ...          ...       ...  ...
+    549  513060      恒生医疗ETF -4.12  0.861  0.905   0.86  0.902 -0.037  47.96  1.57     -   1620502   141454355.0  0.898    290926128    290926128  1.513060   沪A
+    550  515220        煤炭ETF -4.46  2.226  2.394  2.194  2.378 -0.104  14.39  0.98     -   2178176   487720560.0  2.330   3369247992   3369247992  1.515220   沪A
+    551  513000  日经225ETF易方达 -4.49  1.212  1.269   1.21  1.269 -0.057   5.02  2.49     -     25819     3152848.0  1.269     62310617     62310617  1.513000   沪A
+    552  513880     日经225ETF -4.59  1.163  1.224  1.162  1.217 -0.056  16.93  0.94     -     71058     8336846.0  1.219     48811110     48811110  1.513880   沪A
+    553  513520        日经ETF -4.76    1.2  1.217  1.196  1.217  -0.06   27.7  1.79     -    146520    17645828.0  1.260     63464640     63464640  1.513520   沪A
+
+
+    Notes
+    -----
+    无论股票、可转债、期货还是基金。第一列表头始终叫 ``股票代码``
+
+    """
+
+    headers = {'Content-Type': 'application/json', 'token': g_token}
+    url = base_url + 'get_stock_quote_realtime'
+
+    param = {}
+
+    res = requests.post(url=url, headers=headers, data=json.dumps(param))
+
+    if res.ok:
+        return pickle.loads(res.content)
+
+    return res.text
+
 def get_shszhk_capitalflow(exchange_kind = None, start_date = None, end_date = None, fields = None):
     """
     统计时间范围内沪港通、深港通等资金流向数据，以及领涨领跌股，涨跌幅，资金余额等数据信息。数据每日更新。包括科创板；
 
     输入参数：
     :param str exchange_kind : 市场类型，默认"1"
     :param str start_date : 开始日期，默认"five days ago"
```

