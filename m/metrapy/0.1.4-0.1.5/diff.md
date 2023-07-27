# Comparing `tmp/metrapy-0.1.4.tar.gz` & `tmp/metrapy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrapy-0.1.4.tar", last modified: Thu Jul 27 12:12:04 2023, max compression
+gzip compressed data, was "metrapy-0.1.5.tar", last modified: Thu Jul 27 16:55:33 2023, max compression
```

## Comparing `metrapy-0.1.4.tar` & `metrapy-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 12:12:04.860650 metrapy-0.1.4/
--rw-rw-rw-   0        0        0     2670 2023-07-27 12:12:04.859635 metrapy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 12:12:04.822730 metrapy-0.1.4/metrapy/
--rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.4/metrapy/__init__.py
--rw-rw-rw-   0        0        0    13848 2023-07-27 12:11:28.000000 metrapy-0.1.4/metrapy/connector.py
--rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.4/metrapy/defaults.py
--rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.4/metrapy/maps.py
--rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.4/metrapy/sync.py
--rw-rw-rw-   0        0        0      607 2023-07-19 19:33:51.000000 metrapy-0.1.4/metrapy/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 12:12:04.857639 metrapy-0.1.4/metrapy.egg-info/
--rw-rw-rw-   0        0        0     2670 2023-07-27 12:12:04.000000 metrapy-0.1.4/metrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-27 12:12:04.000000 metrapy-0.1.4/metrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 12:12:04.000000 metrapy-0.1.4/metrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-27 12:12:04.000000 metrapy-0.1.4/metrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-27 12:12:04.000000 metrapy-0.1.4/metrapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 12:12:04.860650 metrapy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-07-27 12:11:52.000000 metrapy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:55:33.217841 metrapy-0.1.5/
+-rw-rw-rw-   0        0        0     2670 2023-07-27 16:55:33.217841 metrapy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 16:55:33.144976 metrapy-0.1.5/metrapy/
+-rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.5/metrapy/__init__.py
+-rw-rw-rw-   0        0        0    13885 2023-07-27 16:52:55.000000 metrapy-0.1.5/metrapy/connector.py
+-rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.5/metrapy/defaults.py
+-rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.5/metrapy/maps.py
+-rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.5/metrapy/sync.py
+-rw-rw-rw-   0        0        0      654 2023-07-27 16:54:45.000000 metrapy-0.1.5/metrapy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:55:33.209529 metrapy-0.1.5/metrapy.egg-info/
+-rw-rw-rw-   0        0        0     2670 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 16:55:33.217841 metrapy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-27 16:55:15.000000 metrapy-0.1.5/setup.py
```

### Comparing `metrapy-0.1.4/PKG-INFO` & `metrapy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.4
+Version: 0.1.5
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.4/README.md` & `metrapy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.4/metrapy/connector.py` & `metrapy-0.1.5/metrapy/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def get_account_info(self):
         return mt5.account_info()._asdict()
 
     def get_tickers(self, params={}):
         if "ticker" in params:
             sym = mt5.symbol_info(params["ticker"])
-            return filter_props(sym._asdict(), params["filter_props"])
+            return filter_props(sym._asdict(), params["filter_props"]) if 'filter_props' in params else sym
 
         if "group" in params:
             symbols = mt5.symbols_get(group=params["group"])
         else:
             symbols = mt5.symbols_get()
         
         tickers = []
```

### Comparing `metrapy-0.1.4/metrapy/maps.py` & `metrapy-0.1.5/metrapy/maps.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.4/metrapy/sync.py` & `metrapy-0.1.5/metrapy/sync.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.4/metrapy/utils.py` & `metrapy-0.1.5/metrapy/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 def get_candles_df(candles, timezone=defaults.timezone):
     _candles = pd.DataFrame(
         candles,
         # columns=['Datetime', 'Open', 'High', 'Low', 'Close', 'tick_volume', 'spread', 'real_volume']
     )
 
     _candles["Datetime"] = _candles["time"].map(
-        lambda x: datetime.fromtimestamp(x, timezone)
+        # lambda x: datetime.fromtimestamp(x, timezone)
+        lambda x: datetime.fromtimestamp(x)
     )
 
     _candles = _candles.set_index("Datetime")
 
     return _candles
```

### Comparing `metrapy-0.1.4/metrapy.egg-info/PKG-INFO` & `metrapy-0.1.5/metrapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.4
+Version: 0.1.5
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.4/setup.py` & `metrapy-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metrapy",  # This is the name of the package
-    version="0.1.4",  # The initial release version
+    version="0.1.5",  # The initial release version
     author="pavittarx",  # Full name of the author
     description="batteries included wrapper utility for MetaTrader5's python integration",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

