# Comparing `tmp/empiric_network-1.6.7.tar.gz` & `tmp/empiric_network-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.6.7.tar", max compression
+gzip compressed data, was "empiric_network-1.6.8.tar", max compression
```

## Comparing `empiric_network-1.6.7.tar` & `empiric_network-1.6.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      284 2023-07-26 20:36:55.629989 empiric_network-1.6.7/README.md
--rw-r--r--   0        0        0        0 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/__init__.py
--rw-r--r--   0        0        0      193 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    31179 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4257 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/client.py
--rw-r--r--   0        0        0     2618 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/config.py
--rw-r--r--   0        0        0     3922 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/contract.py
--rw-r--r--   0        0        0    10045 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0    25441 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     9442 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     4177 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     3368 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2262 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/client.py
--rw-r--r--   0        0        0      354 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3826 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     3814 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3754 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3631 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0       71 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/binance.py
--rw-r--r--   0        0        0     3791 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/bybit.py
--rw-r--r--   0        0        0     5675 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/okx.py
--rw-r--r--   0        0        0     4282 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/test.py
--rw-r--r--   0        0        0      668 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1016 2023-07-26 20:36:55.629989 empiric_network-1.6.7/pyproject.toml
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-07-27 17:59:52.841356 empiric_network-1.6.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    31179 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4257 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/client.py
+-rw-r--r--   0        0        0     2618 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/config.py
+-rw-r--r--   0        0        0     3922 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/contract.py
+-rw-r--r--   0        0        0    10045 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25441 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     9442 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     4177 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     3368 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2262 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-07-27 17:59:52.841356 empiric_network-1.6.8/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      113 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/binance.py
+-rw-r--r--   0        0        0     3791 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/bybit.py
+-rw-r--r--   0        0        0     6647 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/okx.py
+-rw-r--r--   0        0        0     4282 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/future_fetchers/test.py
+-rw-r--r--   0        0        0      668 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-07-27 17:59:52.845356 empiric_network-1.6.8/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1016 2023-07-27 17:59:52.845356 empiric_network-1.6.8/pyproject.toml
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.8/PKG-INFO
```

### Comparing `empiric_network-1.6.7/empiric/core/abis/oracle.py` & `empiric_network-1.6.8/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/abis/proxy.py` & `empiric_network-1.6.8/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/abis/publisher_registry.py` & `empiric_network-1.6.8/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/abis/randomness.py` & `empiric_network-1.6.8/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/abis/summary_stats.py` & `empiric_network-1.6.8/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/client.py` & `empiric_network-1.6.8/empiric/core/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/config.py` & `empiric_network-1.6.8/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/contract.py` & `empiric_network-1.6.8/empiric/core/contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/entry.py` & `empiric_network-1.6.8/empiric/core/entry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/mixins/evm.py` & `empiric_network-1.6.8/empiric/core/mixins/evm.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/mixins/nonce.py` & `empiric_network-1.6.8/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/mixins/oracle.py` & `empiric_network-1.6.8/empiric/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.6.8/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/mixins/randomness.py` & `empiric_network-1.6.8/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/mixins/transactions.py` & `empiric_network-1.6.8/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/types.py` & `empiric_network-1.6.8/empiric/core/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/core/utils.py` & `empiric_network-1.6.8/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/assets.py` & `empiric_network-1.6.8/empiric/publisher/assets.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/client.py` & `empiric_network-1.6.8/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/cex.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/defillama.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/kaiko.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/okx.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.6.8/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/future_fetchers/bybit.py` & `empiric_network-1.6.8/empiric/publisher/future_fetchers/bybit.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/future_fetchers/okx.py` & `empiric_network-1.6.8/empiric/publisher/future_fetchers/okx.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,31 @@
                 or result["msg"] == "Instrument ID does not exist"
             ):
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from OKX"
                 )
             return result["data"][0]["expTime"]
 
+    def fetch_sync_expiry_timestamp(self, asset, id):
+        pair = asset["pair"]
+        url = f"{self.TIMESTAMP_URL}?instType=FUTURES&instId={id}"
+        resp = requests.get(url)
+        if resp.status_code == 404:
+            return PublisherFetchError(
+                f"No data found for {'/'.join(pair)} from OKX"
+            )
+        result = resp.json()
+        if (
+            result["code"] == "51001"
+            or result["msg"] == "Instrument ID does not exist"
+        ):
+            return PublisherFetchError(
+                f"No data found for {'/'.join(pair)} from OKX"
+            )
+        return result["data"][0]["expTime"]
     def _construct(self, asset, data, expiry_timestamp) -> List[FutureEntry]:
     
         pair = asset["pair"]
         timestamp = int(int(data["ts"]) / 1000)
         price = float(data["last"])
         price_int = int(price * (10 ** asset["decimals"]))
         pair_id = currency_pair_to_pair_id(*pair)
@@ -84,24 +101,29 @@
                     future_entries.append(self._construct(asset, result['data'][i],expiry_timestamp))
             return future_entries
     
     def _fetch_pair_sync(
         self, asset: EmpiricFutureAsset
     ) -> Union[FutureEntry, PublisherFetchError]:
         pair = asset["pair"]
+        future_entries = []
         url = f"{self.BASE_URL}?instType=FUTURES&uly={pair[0]}-{pair[1]}"
 
         resp = requests.get(url)
         if resp.status_code == 404:
             return PublisherFetchError(f"No data found for {'/'.join(pair)} from OKX")
         result = resp.json(content_type="text/json")
         if result["code"] == "51001" or result["msg"] == "Instrument ID does not exist":
             return PublisherFetchError(f"No data found for {'/'.join(pair)} from OKX")
-
-        return self._construct(asset, result,)
+        result_len = len(result["data"])
+        if result_len > 1:
+            for i in range(0, result_len):
+                expiry_timestamp = self.fetch_sync_expiry_timestamp(asset, result["data"][i]["instId"])
+                future_entries.append(self._construct(asset, result['data'][i],expiry_timestamp))
+        return future_entries
 
     def fetch_sync(self):
         entries = []
         for asset in self.assets:
             if asset["type"] != "FUTURE":
                 logger.debug(f"Skipping OKX for non-future asset {asset}")
                 continue
@@ -112,15 +134,15 @@
                 entries.append(future_entries)
         return entries
 
     async def fetch(self, session: ClientSession):
         entries = []
         for asset in self.assets:
             if asset["type"] != "FUTURE":
-                logger.debug(f"Skipping ByBit for non-future asset {asset}")
+                logger.debug(f"Skipping OKX for non-future asset {asset}")
                 continue
             future_entries = await self._fetch_pair(asset, session)
             if isinstance(future_entries, list):
                 entries.extend(future_entries)
             else:
                 entries.append(future_entries)
         return entries
```

### Comparing `empiric_network-1.6.7/empiric/publisher/future_fetchers/test.py` & `empiric_network-1.6.8/empiric/publisher/future_fetchers/test.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/publisher/types.py` & `empiric_network-1.6.8/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/empiric/test/interface_consistency.py` & `empiric_network-1.6.8/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.7/pyproject.toml` & `empiric_network-1.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.6.7"
+version = "1.6.8"
 authors = ["Pragma <contact@pragmaoracle.com>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragmaoracle.com"
 repository = "https://github.com/Astraly-Labs/Pragma"
 documentation = "https://docs.pragmaoracle.com"
 classifiers = [
```

### Comparing `empiric_network-1.6.7/PKG-INFO` & `empiric_network-1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.6.7
+Version: 1.6.8
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragmaoracle.com
 Author: Pragma
 Author-email: contact@pragmaoracle.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

