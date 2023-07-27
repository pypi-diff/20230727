# Comparing `tmp/stockstats-0.6.0.tar.gz` & `tmp/stockstats-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockstats-0.6.0.tar", last modified: Wed Jun 28 15:31:11 2023, max compression
+gzip compressed data, was "stockstats-0.6.1.tar", last modified: Thu Jul 27 12:53:58 2023, max compression
```

## Comparing `stockstats-0.6.0.tar` & `stockstats-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:31:11.017164 stockstats-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-28 15:31:01.000000 stockstats-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 15:31:01.000000 stockstats-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    34252 2023-06-28 15:31:11.017164 stockstats-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-06-28 15:31:01.000000 stockstats-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 15:31:01.000000 stockstats-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-28 15:31:11.017164 stockstats-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-28 15:31:01.000000 stockstats-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:31:11.017164 stockstats-0.6.0/stockstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34252 2023-06-28 15:31:11.000000 stockstats-0.6.0/stockstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-28 15:31:11.000000 stockstats-0.6.0/stockstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:31:11.000000 stockstats-0.6.0/stockstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-28 15:31:11.000000 stockstats-0.6.0/stockstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 15:31:11.000000 stockstats-0.6.0/stockstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-06-28 15:31:01.000000 stockstats-0.6.0/stockstats.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-28 15:31:01.000000 stockstats-0.6.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:58.055655 stockstats-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-27 12:53:43.000000 stockstats-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 12:53:43.000000 stockstats-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    38602 2023-07-27 12:53:58.055655 stockstats-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37670 2023-07-27 12:53:43.000000 stockstats-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 12:53:43.000000 stockstats-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 12:53:58.055655 stockstats-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-27 12:53:43.000000 stockstats-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:58.055655 stockstats-0.6.1/stockstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38602 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 12:53:58.000000 stockstats-0.6.1/stockstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    65458 2023-07-27 12:53:43.000000 stockstats-0.6.1/stockstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 12:53:43.000000 stockstats-0.6.1/test-requirements.txt
```

### Comparing `stockstats-0.6.0/LICENSE.txt` & `stockstats-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stockstats-0.6.0/PKG-INFO` & `stockstats-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.6.0
+Version: 0.6.1
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.6.0
+VERSION: 0.6.1
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -88,14 +88,20 @@
 * Coppock: Coppock Curve
 * Ichimoku: Ichimoku Cloud
 * CTI: Correlation Trend Indicator
 * LRMA: Linear Regression Moving Average
 * ERI: Elder-Ray Index
 * FTR: the Gaussian Fisher Transform Price Reversals indicator
 * RVGI: Relative Vigor Index
+* Inertia: Inertia Indicator
+* KST: Know Sure Thing
+* PGO: Pretty Good Oscillator
+* PSL: Psychological Line
+* PVO: Percentage Volume Oscillator
+* QQE: Quantitative Qualitative Estimation
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -981,14 +987,119 @@
 
 Examples:
 * `df['rvgi']` retrieves the RVGI line of window 14
 * `df['rvgis']` retrieves the RVGI signal line of window 14
 * `df['rvgi_5']` retrieves the RVGI line of window 5
 * `df['rvgis_5']` retrieves the RVGI signal line of window 5
 
+#### [Inertia Indicator](https://theforexgeek.com/inertia-indicator/)
+
+In financial markets, the concept of inertia was given by Donald Dorsey
+in the 1995 issue of Technical Analysis of Stocks and Commodities
+through the Inertia Indicator. The Inertia Indicator is moment-based
+and is an extension of Dorsey’s Relative Volatility Index (RVI).
+
+Formular:
+* inertia = n periods linear regression of RVGI
+
+Examples:
+* `df['inertia']` retrieves the inertia of 20 periods linear regression of 14 periods RVGI
+* `df['inertia_10']` retrieves the inertia of 10 periods linear regression of 14 periods RVGI
+
+#### [Know Sure Thing (kst)](https://www.investopedia.com/terms/k/know-sure-thing-kst.asp)
+
+The Know Sure Thing (KST) is a momentum oscillator developed by
+Martin Pring to make rate-of-change readings easier for traders
+to interpret.
+
+Formular:
+* KST=(RCMA1×1)+(RCMA2×2) + (RCMA3×3)+(RCMA4×4)
+
+Where:
+* RCMA1=10-period SMA of 10-period ROC
+* RCMA2=10-period SMA of 15-period ROC
+* RCMA3=10-period SMA of 20-period ROC
+* RCMA4=15-period SMA of 30-period ROC
+
+Example:
+* `df['kst']` retrieves the KST.
+
+#### [Pretty Good Oscillator (PGO)](https://library.tradingtechnologies.com/trade/chrt-ti-pretty-good-oscillator.html)
+
+The Pretty Good Oscillator indicator by Mark Johnson measures the 
+distance of the current close from its N-day simple moving average, 
+expressed in terms of an average true range over a similar period.
+
+Formular:
+* PGO = (Close - SMA) / (EMA of TR)
+
+Example:
+* `df['pgo']` retrieves the PGO with default window 14.
+* `df['pgo_10']` retrieves the PGO with window 10.
+
+#### [Psychological Line (PSL)](https://library.tradingtechnologies.com/trade/chrt-ti-psychological-line.html)
+
+The Psychological Line indicator is the ratio of the number of 
+rising periods over the total number of periods.
+
+Formular:
+* PSL = (Number of Rising Periods) / (Total Number of Periods) * 100
+
+Example:
+* `df['psl']` retrieves the PSL with default window 12.
+* `df['psl_10']` retrieves the PSL with window 10.
+* `df['high_12_psl']` retrieves the PSL of high price with window 10.
+
+#### [Percentage Volume Oscillator(PVO)](https://school.stockcharts.com/doku.php?id=technical_indicators:percentage_volume_oscillator_pvo)
+
+The Percentage Volume Oscillator (PVO) is a momentum oscillator for volume. 
+The PVO measures the difference between two volume-based moving averages as
+a percentage of the larger moving average.
+
+Formular: 
+
+* Percentage Volume Oscillator (PVO): 
+  ((12-day EMA of Volume - 26-day EMA of Volume)/26-day EMA of Volume) x 100
+* Signal Line: 9-day EMA of PVO
+* PVO Histogram: PVO - Signal Line
+
+Example:
+* `df['pvo']` derives from the difference of 2 exponential moving average.
+* `df['pvos]` is the signal line.
+* `df['pvoh']` is he histogram line.
+
+The period of short, long EMA and signal line can be tuned with 
+`set_dft_window('pvo', (short, long, signal))`.  The default
+windows are 12 and 26 and 9.
+
+#### [Quantitative Qualitative Estimation(QQE)](https://www.tradingview.com/script/0vn4HZ7O-Quantitative-Qualitative-Estimation-QQE/)
+
+The Qualitative Quantitative Estimation (QQE) indicator works like a smoother 
+version of the popular Relative Strength Index (RSI) indicator. QQE expands 
+on RSI by adding two volatility based trailing stop lines. These trailing 
+stop lines are composed of a fast and a slow moving Average True Range (ATR). 
+These ATR lines are smoothed making this indicator less susceptible to short 
+term volatility.
+
+Implementation reference:
+https://github.com/twopirllc/pandas-ta/blob/main/pandas_ta/momentum/qqe.py
+
+Example:
+* `df['qqe']` retrieves the QQE with RSI window 14, MA window 5.
+* `df['qqel']` retrieves the QQE long
+* `df['qqes']` retrieves the QQE short
+* `df['qqe_10,4']` retrieves the QQE with RSI window 10, MA window 4
+* `df['qqel_10,4']` retrieves the QQE long with customized windows.
+  Initialized by retrieving `df['qqe_10,4']`
+* `df['qqes_10,4']` retrieves the QQE short with customized windows
+  Initialized by retrieving `df['qqe_10,4']`
+
+The period of short, long EMA and signal line can be tuned with 
+`set_dft_window('qqe', (rsi, rsi_ma))`.  The default windows are 14 and 5.
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

### Comparing `stockstats-0.6.0/README.md` & `stockstats-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.6.0
+VERSION: 0.6.1
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -63,14 +63,20 @@
 * Coppock: Coppock Curve
 * Ichimoku: Ichimoku Cloud
 * CTI: Correlation Trend Indicator
 * LRMA: Linear Regression Moving Average
 * ERI: Elder-Ray Index
 * FTR: the Gaussian Fisher Transform Price Reversals indicator
 * RVGI: Relative Vigor Index
+* Inertia: Inertia Indicator
+* KST: Know Sure Thing
+* PGO: Pretty Good Oscillator
+* PSL: Psychological Line
+* PVO: Percentage Volume Oscillator
+* QQE: Quantitative Qualitative Estimation
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -956,14 +962,119 @@
 
 Examples:
 * `df['rvgi']` retrieves the RVGI line of window 14
 * `df['rvgis']` retrieves the RVGI signal line of window 14
 * `df['rvgi_5']` retrieves the RVGI line of window 5
 * `df['rvgis_5']` retrieves the RVGI signal line of window 5
 
+#### [Inertia Indicator](https://theforexgeek.com/inertia-indicator/)
+
+In financial markets, the concept of inertia was given by Donald Dorsey
+in the 1995 issue of Technical Analysis of Stocks and Commodities
+through the Inertia Indicator. The Inertia Indicator is moment-based
+and is an extension of Dorsey’s Relative Volatility Index (RVI).
+
+Formular:
+* inertia = n periods linear regression of RVGI
+
+Examples:
+* `df['inertia']` retrieves the inertia of 20 periods linear regression of 14 periods RVGI
+* `df['inertia_10']` retrieves the inertia of 10 periods linear regression of 14 periods RVGI
+
+#### [Know Sure Thing (kst)](https://www.investopedia.com/terms/k/know-sure-thing-kst.asp)
+
+The Know Sure Thing (KST) is a momentum oscillator developed by
+Martin Pring to make rate-of-change readings easier for traders
+to interpret.
+
+Formular:
+* KST=(RCMA1×1)+(RCMA2×2) + (RCMA3×3)+(RCMA4×4)
+
+Where:
+* RCMA1=10-period SMA of 10-period ROC
+* RCMA2=10-period SMA of 15-period ROC
+* RCMA3=10-period SMA of 20-period ROC
+* RCMA4=15-period SMA of 30-period ROC
+
+Example:
+* `df['kst']` retrieves the KST.
+
+#### [Pretty Good Oscillator (PGO)](https://library.tradingtechnologies.com/trade/chrt-ti-pretty-good-oscillator.html)
+
+The Pretty Good Oscillator indicator by Mark Johnson measures the 
+distance of the current close from its N-day simple moving average, 
+expressed in terms of an average true range over a similar period.
+
+Formular:
+* PGO = (Close - SMA) / (EMA of TR)
+
+Example:
+* `df['pgo']` retrieves the PGO with default window 14.
+* `df['pgo_10']` retrieves the PGO with window 10.
+
+#### [Psychological Line (PSL)](https://library.tradingtechnologies.com/trade/chrt-ti-psychological-line.html)
+
+The Psychological Line indicator is the ratio of the number of 
+rising periods over the total number of periods.
+
+Formular:
+* PSL = (Number of Rising Periods) / (Total Number of Periods) * 100
+
+Example:
+* `df['psl']` retrieves the PSL with default window 12.
+* `df['psl_10']` retrieves the PSL with window 10.
+* `df['high_12_psl']` retrieves the PSL of high price with window 10.
+
+#### [Percentage Volume Oscillator(PVO)](https://school.stockcharts.com/doku.php?id=technical_indicators:percentage_volume_oscillator_pvo)
+
+The Percentage Volume Oscillator (PVO) is a momentum oscillator for volume. 
+The PVO measures the difference between two volume-based moving averages as
+a percentage of the larger moving average.
+
+Formular: 
+
+* Percentage Volume Oscillator (PVO): 
+  ((12-day EMA of Volume - 26-day EMA of Volume)/26-day EMA of Volume) x 100
+* Signal Line: 9-day EMA of PVO
+* PVO Histogram: PVO - Signal Line
+
+Example:
+* `df['pvo']` derives from the difference of 2 exponential moving average.
+* `df['pvos]` is the signal line.
+* `df['pvoh']` is he histogram line.
+
+The period of short, long EMA and signal line can be tuned with 
+`set_dft_window('pvo', (short, long, signal))`.  The default
+windows are 12 and 26 and 9.
+
+#### [Quantitative Qualitative Estimation(QQE)](https://www.tradingview.com/script/0vn4HZ7O-Quantitative-Qualitative-Estimation-QQE/)
+
+The Qualitative Quantitative Estimation (QQE) indicator works like a smoother 
+version of the popular Relative Strength Index (RSI) indicator. QQE expands 
+on RSI by adding two volatility based trailing stop lines. These trailing 
+stop lines are composed of a fast and a slow moving Average True Range (ATR). 
+These ATR lines are smoothed making this indicator less susceptible to short 
+term volatility.
+
+Implementation reference:
+https://github.com/twopirllc/pandas-ta/blob/main/pandas_ta/momentum/qqe.py
+
+Example:
+* `df['qqe']` retrieves the QQE with RSI window 14, MA window 5.
+* `df['qqel']` retrieves the QQE long
+* `df['qqes']` retrieves the QQE short
+* `df['qqe_10,4']` retrieves the QQE with RSI window 10, MA window 4
+* `df['qqel_10,4']` retrieves the QQE long with customized windows.
+  Initialized by retrieving `df['qqe_10,4']`
+* `df['qqes_10,4']` retrieves the QQE short with customized windows
+  Initialized by retrieving `df['qqe_10,4']`
+
+The period of short, long EMA and signal line can be tuned with 
+`set_dft_window('qqe', (rsi, rsi_ma))`.  The default windows are 14 and 5.
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

### Comparing `stockstats-0.6.0/setup.py` & `stockstats-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `stockstats-0.6.0/stockstats.egg-info/PKG-INFO` & `stockstats-0.6.1/stockstats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.6.0
+Version: 0.6.1
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.6.0
+VERSION: 0.6.1
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -88,14 +88,20 @@
 * Coppock: Coppock Curve
 * Ichimoku: Ichimoku Cloud
 * CTI: Correlation Trend Indicator
 * LRMA: Linear Regression Moving Average
 * ERI: Elder-Ray Index
 * FTR: the Gaussian Fisher Transform Price Reversals indicator
 * RVGI: Relative Vigor Index
+* Inertia: Inertia Indicator
+* KST: Know Sure Thing
+* PGO: Pretty Good Oscillator
+* PSL: Psychological Line
+* PVO: Percentage Volume Oscillator
+* QQE: Quantitative Qualitative Estimation
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -981,14 +987,119 @@
 
 Examples:
 * `df['rvgi']` retrieves the RVGI line of window 14
 * `df['rvgis']` retrieves the RVGI signal line of window 14
 * `df['rvgi_5']` retrieves the RVGI line of window 5
 * `df['rvgis_5']` retrieves the RVGI signal line of window 5
 
+#### [Inertia Indicator](https://theforexgeek.com/inertia-indicator/)
+
+In financial markets, the concept of inertia was given by Donald Dorsey
+in the 1995 issue of Technical Analysis of Stocks and Commodities
+through the Inertia Indicator. The Inertia Indicator is moment-based
+and is an extension of Dorsey’s Relative Volatility Index (RVI).
+
+Formular:
+* inertia = n periods linear regression of RVGI
+
+Examples:
+* `df['inertia']` retrieves the inertia of 20 periods linear regression of 14 periods RVGI
+* `df['inertia_10']` retrieves the inertia of 10 periods linear regression of 14 periods RVGI
+
+#### [Know Sure Thing (kst)](https://www.investopedia.com/terms/k/know-sure-thing-kst.asp)
+
+The Know Sure Thing (KST) is a momentum oscillator developed by
+Martin Pring to make rate-of-change readings easier for traders
+to interpret.
+
+Formular:
+* KST=(RCMA1×1)+(RCMA2×2) + (RCMA3×3)+(RCMA4×4)
+
+Where:
+* RCMA1=10-period SMA of 10-period ROC
+* RCMA2=10-period SMA of 15-period ROC
+* RCMA3=10-period SMA of 20-period ROC
+* RCMA4=15-period SMA of 30-period ROC
+
+Example:
+* `df['kst']` retrieves the KST.
+
+#### [Pretty Good Oscillator (PGO)](https://library.tradingtechnologies.com/trade/chrt-ti-pretty-good-oscillator.html)
+
+The Pretty Good Oscillator indicator by Mark Johnson measures the 
+distance of the current close from its N-day simple moving average, 
+expressed in terms of an average true range over a similar period.
+
+Formular:
+* PGO = (Close - SMA) / (EMA of TR)
+
+Example:
+* `df['pgo']` retrieves the PGO with default window 14.
+* `df['pgo_10']` retrieves the PGO with window 10.
+
+#### [Psychological Line (PSL)](https://library.tradingtechnologies.com/trade/chrt-ti-psychological-line.html)
+
+The Psychological Line indicator is the ratio of the number of 
+rising periods over the total number of periods.
+
+Formular:
+* PSL = (Number of Rising Periods) / (Total Number of Periods) * 100
+
+Example:
+* `df['psl']` retrieves the PSL with default window 12.
+* `df['psl_10']` retrieves the PSL with window 10.
+* `df['high_12_psl']` retrieves the PSL of high price with window 10.
+
+#### [Percentage Volume Oscillator(PVO)](https://school.stockcharts.com/doku.php?id=technical_indicators:percentage_volume_oscillator_pvo)
+
+The Percentage Volume Oscillator (PVO) is a momentum oscillator for volume. 
+The PVO measures the difference between two volume-based moving averages as
+a percentage of the larger moving average.
+
+Formular: 
+
+* Percentage Volume Oscillator (PVO): 
+  ((12-day EMA of Volume - 26-day EMA of Volume)/26-day EMA of Volume) x 100
+* Signal Line: 9-day EMA of PVO
+* PVO Histogram: PVO - Signal Line
+
+Example:
+* `df['pvo']` derives from the difference of 2 exponential moving average.
+* `df['pvos]` is the signal line.
+* `df['pvoh']` is he histogram line.
+
+The period of short, long EMA and signal line can be tuned with 
+`set_dft_window('pvo', (short, long, signal))`.  The default
+windows are 12 and 26 and 9.
+
+#### [Quantitative Qualitative Estimation(QQE)](https://www.tradingview.com/script/0vn4HZ7O-Quantitative-Qualitative-Estimation-QQE/)
+
+The Qualitative Quantitative Estimation (QQE) indicator works like a smoother 
+version of the popular Relative Strength Index (RSI) indicator. QQE expands 
+on RSI by adding two volatility based trailing stop lines. These trailing 
+stop lines are composed of a fast and a slow moving Average True Range (ATR). 
+These ATR lines are smoothed making this indicator less susceptible to short 
+term volatility.
+
+Implementation reference:
+https://github.com/twopirllc/pandas-ta/blob/main/pandas_ta/momentum/qqe.py
+
+Example:
+* `df['qqe']` retrieves the QQE with RSI window 14, MA window 5.
+* `df['qqel']` retrieves the QQE long
+* `df['qqes']` retrieves the QQE short
+* `df['qqe_10,4']` retrieves the QQE with RSI window 10, MA window 4
+* `df['qqel_10,4']` retrieves the QQE long with customized windows.
+  Initialized by retrieving `df['qqe_10,4']`
+* `df['qqes_10,4']` retrieves the QQE short with customized windows
+  Initialized by retrieving `df['qqe_10,4']`
+
+The period of short, long EMA and signal line can be tuned with 
+`set_dft_window('qqe', (rsi, rsi_ma))`.  The default windows are 14 and 5.
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

### Comparing `stockstats-0.6.0/stockstats.py` & `stockstats-0.6.1/stockstats.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 # ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import unicode_literals
 
+import functools
 import itertools
 import re
 from typing import Optional, Callable, Union
 
 import numpy as np
 import pandas as pd
 
@@ -56,25 +57,30 @@
     'cr': 26,
     'cti': 12,
     'dma': (10, 50),
     'eri': 13,
     'eribear': 13,
     'eribull': 13,
     'ichimoku': (9, 26, 52),
+    'inertia': (20, 14),
     'ftr': 9,
     'kama': (10, 5, 34),  # window, fast, slow
     'kdjd': 9,
     'kdjj': 9,
     'kdjk': 9,
     'ker': 10,
     'macd': (12, 26, 9),  # short, long, signal
     'mfi': 14,
     'ndi': 14,
     'pdi': 14,
+    'pgo': 14,
     'ppo': (12, 26, 9),  # short, long, signal
+    'pvo': (12, 26, 9),  # short, long, signal
+    'psl': 12,
+    'qqe': (14, 5),  # rsi, rsi ema
     'rsi': 14,
     'rsv': 9,
     'rvgi': 14,
     'stochrsi': 14,
     'supertrend': 14,
     'tema': 5,
     'trix': 12,
@@ -93,14 +99,15 @@
 
 _dft_column = {
     # sort alphabetically
     'cti': 'close',
     'dma': 'close',
     'kama': 'close',
     'ker': 'close',
+    'psl': 'close',
     'tema': 'close',
     'trix': 'close',
 }
 
 
 def dft_windows(name: str) -> Optional[str]:
     if name not in _dft_windows:
@@ -446,15 +453,16 @@
         This value is essential for calculating KDJs
         Current day is included in N
 
         """
         self[meta.name] = self._rsv(meta.int)
 
     def _rsi(self, window) -> pd.Series:
-        change = self._delta(self['close'], -1)
+        change = self.close.diff()
+        change.iloc[0] = 0
         close_pm = (change + change.abs()) / 2
         close_nm = (-change + change.abs()) / 2
         p_ema = self.smma(close_pm, window)
         n_ema = self.smma(close_nm, window)
 
         rs = p_ema / n_ema
         return 100 - 100 / (1.0 + rs)
@@ -989,19 +997,19 @@
         Where:
         * PriceP: the price of the current period
         * PricePn: the price of the n periods ago
         """
         self[meta.name] = self.roc(self[meta.column], meta.int)
 
     @staticmethod
-    def ema(series, window, *, adjust=True):
+    def ema(series, window, *, adjust=True, min_periods=1):
         return series.ewm(
             ignore_na=False,
             span=window,
-            min_periods=1,
+            min_periods=min_periods,
             adjust=adjust).mean()
 
     @staticmethod
     def _rolling(series: pd.Series, window: int):
         return series.rolling(window, min_periods=1, center=False)
 
     @classmethod
@@ -1112,33 +1120,58 @@
         macd = meta.name
         macds = meta.name_ex('s')
         macdh = meta.name_ex('h')
         self[macd] = ema_short - ema_long
         self[macds] = self.ema(self[macd], signal_w)
         self[macdh] = self[macd] - self[macds]
 
+    def _ppo_and_pvo(self, name: str, col_name: str, meta: _Meta):
+        volume = self[col_name]
+        short_w, long_w, signal_w = meta.int0, meta.int1, meta.int2
+        pvo_short = self.ema(volume, short_w)
+        pvo_long = self.ema(volume, long_w)
+        self[name] = (pvo_short - pvo_long) / pvo_long * 100
+        self[f'{name}s'] = self.ema(self[name], signal_w)
+        self[f'{name}h'] = self[name] - self[f'{name}s']
+
+    def _get_pvo(self, meta: _Meta):
+        """ Percentage Volume Oscillator
+
+        The Percentage Volume Oscillator (PVO) is a momentum oscillator for
+        volume.  The PVO measures the difference between two volume-based
+        moving averages as a percentage of the larger moving average.
+
+        https://school.stockcharts.com/doku.php?id=technical_indicators:percentage_volume_oscillator_pvo
+
+        Percentage Volume Oscillator (PVO):
+            {(12_EOV - 26_EOV)/26_EOV} x 100
+
+        Where:
+        * 12_EOV is the 12-day EMA of Volume
+        * 26_EOV is the 26-day EMA of Volume
+
+        Signal Line: 9-day EMA of PVO
+
+        PVO Histogram: PVO - Signal Line
+        """
+        return self._ppo_and_pvo('pvo', 'volume', meta)
+
     def _get_ppo(self, meta: _Meta):
         """ Percentage Price Oscillator
 
         https://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:price_oscillators_ppo
 
         Percentage Price Oscillator (PPO):
             {(12-day EMA - 26-day EMA)/26-day EMA} x 100
 
         Signal Line: 9-day EMA of PPO
 
         PPO Histogram: PPO - Signal Line
         """
-        close = self['close']
-        short_w, long_w, signal_w = meta.int0, meta.int1, meta.int2
-        ppo_short = self.ema(close, short_w)
-        ppo_long = self.ema(close, long_w)
-        self['ppo'] = (ppo_short - ppo_long) / ppo_long * 100
-        self['ppos'] = self.ema(self['ppo'], signal_w)
-        self['ppoh'] = self['ppo'] - self['ppos']
+        return self._ppo_and_pvo('ppo', 'close', meta)
 
     def _eri(self, window):
         ema = self.ema(self['close'], window, adjust=False)
         bull = self['high'] - ema
         bear = self['low'] - ema
         return bull, bear
 
@@ -1530,14 +1563,191 @@
         rvgi = self._rvgi(meta.int)
         rvgi.iloc[:3] = 0.0
         rvgi_s = self.sym_wma4(rvgi)
         rvgi_s.iloc[:6] = 0.0
         self[meta.name] = rvgi
         self[meta.name_ex('s')] = rvgi_s
 
+    def _inertia(self, window: int, rvgi_window: int) -> pd.Series:
+        """ Inertia Indicator
+
+        https://theforexgeek.com/inertia-indicator/
+
+        In financial markets, the concept of inertia was given by Donald Dorsey
+        in the 1995 issue of Technical Analysis of Stocks and Commodities
+        through the Inertia Indicator. The Inertia Indicator is moment-based
+        and is an extension of Dorsey’s Relative Volatility Index (RVI).
+        """
+        rvgi = self._rvgi(rvgi_window)
+        value = self.linear_reg(rvgi, window)
+        value.iloc[:max(window, rvgi_window) + 2] = 0
+        return value
+
+    def _get_inertia(self, meta: _Meta):
+        value = self._inertia(meta.int0, meta.int1)
+        self[meta.name] = value
+
+    def _kst(self) -> pd.Series:
+        """ Know Sure Thing (kst)
+
+        https://www.investopedia.com/terms/k/know-sure-thing-kst.asp
+
+        The Know Sure Thing (KST) is a momentum oscillator developed by
+        Martin Pring to make rate-of-change readings easier for traders
+        to interpret.
+
+        Formular:
+        * KST=(RCMA #1×1)+(RCMA #2×2) + (RCMA #3×3)+(RCMA #4×4)
+
+        where:
+        * RCMA #1=10-period SMA of 10-period ROC
+        * RCMA #2=10-period SMA of 15-period ROC
+        * RCMA #3=10-period SMA of 20-period ROC
+        * RCMA #4=15-period SMA of 30-period ROC
+        """
+        ma1 = self.sma(self.roc(self.close, 10), 10)
+        ma2 = self.sma(self.roc(self.close, 15), 10)
+        ma3 = self.sma(self.roc(self.close, 20), 10)
+        ma4 = self.sma(self.roc(self.close, 30), 15)
+        return ma1 + ma2 * 2 + ma3 * 3 + ma4 * 4
+
+    def _get_kst(self, meta: _Meta):
+        self[meta.name] = self._kst()
+
+    def _pgo(self, window: int) -> pd.Series:
+        """ Pretty Good Oscillator (PGO)
+
+        https://library.tradingtechnologies.com/trade/chrt-ti-pretty-good-oscillator.html
+
+        The Pretty Good Oscillator indicator by Mark Johnson measures the
+        distance of the current close from its N-day simple moving average,
+        expressed in terms of an average true range over a similar period.
+
+        Formular:
+        * PGO = (Close - SMA) / (EMA of TR)
+
+        Where:
+        * SMA = Simple Moving Average of Close over N periods
+        * EMA of TR = Exponential Moving Average of True Range over N periods
+        """
+        up = self.close - self.sma(self.close, window)
+        down = self.ema(self._tr(), window)
+        return up / down
+
+    def _get_pgo(self, meta: _Meta):
+        self[meta.name] = self._pgo(meta.int)
+
+    def _psl(self, col_name: str, window: int) -> pd.Series:
+        """ Psychological Line (PSL)
+
+        The Psychological Line indicator is the ratio of the number of
+        rising periods over the total number of periods.
+
+        https://library.tradingtechnologies.com/trade/chrt-ti-psychological-line.html
+
+        Formular:
+        * PSL = (Number of Rising Periods) / (Total Number of Periods) * 100
+
+        Example:
+        * `df['psl']` retrieves the PSL with default window 12.
+        * `df['psl_10']` retrieves the PSL with window 10.
+        * `df['high_12_psl']` retrieves the PSL of high price with window 10.
+        """
+        col_diff = self._col_diff(col_name)
+        pos = col_diff > 0
+        return self.mov_sum(pos, window) / window * 100
+
+    def _get_psl(self, meta: _Meta):
+        self[meta.name] = self._psl(meta.column, meta.int)
+
+    def _get_qqe(self, meta: _Meta):
+        """ QQE (Quantitative Qualitative Estimation)
+
+        https://www.tradingview.com/script/0vn4HZ7O-Quantitative-Qualitative-Estimation-QQE/
+
+        The Qualitative Quantitative Estimation (QQE) indicator works like a
+        smoother version of the popular Relative Strength Index (RSI)
+        indicator. QQE expands on RSI by adding two volatility based trailing
+        stop lines. These trailing stop lines are composed of a fast and a
+        slow moving Average True Range (ATR).  These ATR lines are smoothed
+        making this indicator less susceptible to short term volatility.
+
+        Implementation reference:
+        https://github.com/twopirllc/pandas-ta/blob/main/pandas_ta/momentum/qqe.py
+
+        """
+        rsi_window = meta.int0
+        rsi_ma_window = meta.int1
+        factor = 4.236
+        wilder_window = rsi_window * 2 - 1
+        ema = functools.partial(self.ema, adjust=False)
+
+        rsi = self._rsi(rsi_window)
+        rsi.iloc[:rsi_window] = np.nan
+        rsi_ma = ema(rsi, rsi_ma_window)
+        tr = rsi_ma.diff().abs()
+        tr_ma = ema(tr, wilder_window)
+        tr_ma_ma = ema(tr_ma, wilder_window) * factor
+
+        upper = list(rsi_ma + tr_ma_ma)
+        lower = list(rsi_ma - tr_ma_ma)
+        rsi_ma = list(rsi_ma)
+
+        size = self.close.size
+        long = [0] * size
+        short = [0] * size
+        trend = [1] * size
+        qqe = [rsi_ma[0]] * size
+        qqe_long = [np.nan] * size
+        qqe_short = [np.nan] * size
+
+        for i in range(1, size):
+            c_rsi, p_rsi = rsi_ma[i], rsi_ma[i - 1]
+            c_long, p_long = long[i - 1], long[i - 2]
+            c_short, p_short = short[i - 1], short[i - 2]
+
+            # Long Line
+            if p_rsi > c_long and c_rsi > c_long:
+                long[i] = max(c_long, lower[i])
+            else:
+                long[i] = lower[i]
+
+            # Short Line
+            if p_rsi < c_short and c_rsi < c_short:
+                short[i] = min(c_short, upper[i])
+            else:
+                short[i] = upper[i]
+
+            # Trend & QQE Calculation
+            # Long: Current RSI_MA value Crosses the Prior Short Line Value
+            # Short: Current RSI_MA Crosses the Prior Long Line Value
+            rsi_ux_short = c_rsi > c_short and p_rsi < p_short
+            rsi_dx_short = c_rsi <= c_short and p_rsi >= p_short
+            rsi_ux_long = c_rsi > c_long and p_rsi < p_long
+            rsi_dx_long = c_rsi <= c_long and p_rsi >= p_long
+            if rsi_ux_short or rsi_dx_short:
+                trend[i] = 1
+                qqe[i] = qqe_long[i] = long[i]
+            elif rsi_ux_long or rsi_dx_long:
+                trend[i] = -1
+                qqe[i] = qqe_short[i] = short[i]
+            else:
+                trend[i] = trend[i - 1]
+                if trend[i] == 1:
+                    qqe[i] = qqe_long[i] = long[i]
+                else:
+                    qqe[i] = qqe_short[i] = short[i]
+
+        self[meta.name] = self.to_series(qqe)
+        self[meta.name_ex('l')] = self.to_series(qqe_long)
+        self[meta.name_ex('s')] = self.to_series(qqe_short)
+
+    def to_series(self, arr: list):
+        return pd.Series(arr, index=self.close.index).fillna(0)
+
     @staticmethod
     def parse_column_name(name):
         m = re.match(r'(.*)_([\d\-+~,.]+)_(\w+)', name)
         ret = (None,)
         if m is None:
             m = re.match(r'(.*)_([\d\-+~,]+)', name)
             if m is not None:
@@ -1627,62 +1837,46 @@
         """
         head = self.head(n).index
         ret = self.drop(head, inplace=inplace)
         if inplace is True:
             return self
         return wrap(ret)
 
+    def _get_handler(self, name: str):
+        return getattr(self, f'_get_{name}')
+
     @property
     def handler(self):
-        return {
-            ('change',): self._get_change,
-            ('rsi',): self._get_rsi,
-            ('stochrsi',): self._get_stochrsi,
+        ret = {
             ('rate',): self._get_rate,
             ('middle',): self._get_middle,
             ('tp',): self._get_tp,
             ('boll', 'boll_ub', 'boll_lb'): self._get_boll,
             ('macd', 'macds', 'macdh'): self._get_macd,
+            ('pvo', 'pvos', 'pvoh'): self._get_pvo,
             ('ppo', 'ppos', 'ppoh'): self._get_ppo,
-            ('kdjk',): self._get_kdjk,
-            ('kdjd',): self._get_kdjd,
-            ('kdjj',): self._get_kdjj,
-            ('rsv',): self._get_rsv,
+            ('qqe', 'qqel', 'qqes'): self._get_qqe,
             ('cr', 'cr-ma1', 'cr-ma2', 'cr-ma3'): self._get_cr,
-            ('cci',): self._get_cci,
             ('tr',): self._get_tr,
-            ('atr',): self._get_atr,
-            ('pdi',): self._get_pdi,
-            ('ndi',): self._get_ndi,
             ('dx', 'adx', 'adxr'): self._get_dmi,
-            ('trix',): self._get_trix,
-            ('tema',): self._get_tema,
-            ('vr',): self._get_vr,
-            ('dma',): self._get_dma,
-            ('vwma',): self._get_vwma,
-            ('chop',): self._get_chop,
             ('log-ret',): self._get_log_ret,
-            ('mfi',): self._get_mfi,
             ('wt1', 'wt2'): self._get_wt,
-            ('wr',): self._get_wr,
             ('supertrend',
              'supertrend_lb',
              'supertrend_ub'): self._get_supertrend,
-            ('aroon',): self._get_aroon,
-            ('ao',): self._get_ao,
             ('bop',): self._get_bop,
-            ('cmo',): self._get_cmo,
-            ('coppock',): self._get_coppock,
-            ('ichimoku',): self._get_ichimoku,
             ('cti',): self._get_cti,
-            ('ker',): self._get_ker,
             ('eribull', 'eribear'): self._get_eri,
-            ('ftr',): self._get_ftr,
             ('rvgi', 'rvgis'): self._get_rvgi,
+            ('kst',): self._get_kst,
         }
+        for k in _dft_windows.keys():
+            if k not in ret:
+                ret[k] = self._get_handler(k)
+        return ret
 
     def __init_not_exist_column(self, key):
         for names, handler in self.handler.items():
             if key in names:
                 return _call_handler(handler)
 
         if key.endswith('_delta'):
@@ -1696,15 +1890,15 @@
             elif len(ret) == 2:
                 name, n = ret
                 col = None
             else:
                 raise UserWarning("Invalid number of return arguments "
                                   f"after parsing column name: '{key}'")
             meta = _Meta(name, windows=n, column=col)
-            getattr(self, f'_get_{name}')(meta)
+            self._get_handler(name)(meta)
 
     def __init_column(self, key):
         if key not in self:
             if len(self) == 0:
                 self[key] = []
             else:
                 self.__init_not_exist_column(key)
```

