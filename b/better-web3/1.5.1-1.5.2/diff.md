# Comparing `tmp/better_web3-1.5.1.tar.gz` & `tmp/better_web3-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-1.5.1.tar", max compression
+gzip compressed data, was "better_web3-1.5.2.tar", max compression
```

## Comparing `better_web3-1.5.1.tar` & `better_web3-1.5.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      359 2023-07-26 14:40:25.024000 better_web3-1.5.1/better_web3/__init__.py
--rw-r--r--   0        0        0    10461 2023-07-17 08:28:26.368000 better_web3-1.5.1/better_web3/batch_call.py
--rw-r--r--   0        0        0    14931 2023-07-26 13:56:34.907000 better_web3-1.5.1/better_web3/chain.py
--rw-r--r--   0        0        0      251 2023-07-07 12:10:25.885000 better_web3-1.5.1/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      525 2023-07-11 06:39:31.842000 better_web3-1.5.1/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      687 2023-07-11 06:39:33.730000 better_web3-1.5.1/better_web3/contract/__pycache__/_abi.cpython-311.pyc
--rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.5.1/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0     2938 2023-07-11 06:39:31.913000 better_web3-1.5.1/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     1938 2023-07-11 06:39:34.027000 better_web3-1.5.1/better_web3/contract/__pycache__/disperse.cpython-311.pyc
--rw-r--r--   0        0        0     3687 2023-07-11 06:39:34.086000 better_web3-1.5.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     5293 2023-07-11 06:39:34.163000 better_web3-1.5.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     9601 2023-07-11 06:39:33.679000 better_web3-1.5.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0      352 2023-07-07 12:03:06.296000 better_web3-1.5.1/better_web3/contract/_abi.py
--rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.5.1/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-1.5.1/better_web3/contract/abi/disperse.json
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.5.1/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.5.1/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.5.1/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.5.1/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0     1264 2023-07-10 08:18:27.356000 better_web3-1.5.1/better_web3/contract/contract.py
--rw-r--r--   0        0        0      974 2023-07-07 12:13:30.821000 better_web3-1.5.1/better_web3/contract/disperse.py
--rw-r--r--   0        0        0     1747 2023-07-07 20:11:33.426000 better_web3-1.5.1/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     2876 2023-07-07 20:11:33.364000 better_web3-1.5.1/better_web3/contract/erc721.py
--rw-r--r--   0        0        0     6201 2023-07-07 12:07:18.259000 better_web3-1.5.1/better_web3/contract/multicall.py
--rw-r--r--   0        0        0     4059 2023-07-26 11:29:17.505000 better_web3-1.5.1/better_web3/proxy.py
--rw-r--r--   0        0        0      730 2023-07-17 08:28:26.473000 better_web3-1.5.1/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-07-17 08:28:28.447000 better_web3-1.5.1/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4132 2023-07-17 08:28:28.496000 better_web3-1.5.1/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.5.1/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     1398 2023-07-11 06:39:33.869000 better_web3-1.5.1/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0     2131 2023-07-17 08:28:26.617000 better_web3-1.5.1/better_web3/utils/eth.py
--rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.5.1/better_web3/utils/file.py
--rw-r--r--   0        0        0      663 2023-07-07 20:05:19.087000 better_web3-1.5.1/better_web3/utils/other.py
--rw-r--r--   0        0        0     3227 2023-07-26 11:29:17.244000 better_web3-1.5.1/better_web3/wallet.py
--rw-r--r--   0        0        0      412 2023-07-26 14:41:16.097000 better_web3-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      479 2023-07-07 17:47:32.398000 better_web3-1.5.1/README.md
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 better_web3-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      359 2023-07-26 14:40:25.024000 better_web3-1.5.2/better_web3/__init__.py
+-rw-r--r--   0        0        0    10370 2023-07-26 14:53:35.350000 better_web3-1.5.2/better_web3/batch_call.py
+-rw-r--r--   0        0        0    14869 2023-07-26 15:28:37.218000 better_web3-1.5.2/better_web3/chain.py
+-rw-r--r--   0        0        0      251 2023-07-07 12:10:25.885000 better_web3-1.5.2/better_web3/contract/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-11 06:39:31.842000 better_web3-1.5.2/better_web3/contract/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      687 2023-07-11 06:39:33.730000 better_web3-1.5.2/better_web3/contract/__pycache__/_abi.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.5.2/better_web3/contract/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0     2938 2023-07-11 06:39:31.913000 better_web3-1.5.2/better_web3/contract/__pycache__/contract.cpython-311.pyc
+-rw-r--r--   0        0        0     1938 2023-07-11 06:39:34.027000 better_web3-1.5.2/better_web3/contract/__pycache__/disperse.cpython-311.pyc
+-rw-r--r--   0        0        0     3687 2023-07-11 06:39:34.086000 better_web3-1.5.2/better_web3/contract/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     5293 2023-07-11 06:39:34.163000 better_web3-1.5.2/better_web3/contract/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     9601 2023-07-11 06:39:33.679000 better_web3-1.5.2/better_web3/contract/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0      352 2023-07-07 12:03:06.296000 better_web3-1.5.2/better_web3/contract/_abi.py
+-rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.5.2/better_web3/contract/_paths.py
+-rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-1.5.2/better_web3/contract/abi/disperse.json
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.5.2/better_web3/contract/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.5.2/better_web3/contract/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.5.2/better_web3/contract/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.5.2/better_web3/contract/abi/multicall_v3.json
+-rw-r--r--   0        0        0     1264 2023-07-10 08:18:27.356000 better_web3-1.5.2/better_web3/contract/contract.py
+-rw-r--r--   0        0        0      974 2023-07-07 12:13:30.821000 better_web3-1.5.2/better_web3/contract/disperse.py
+-rw-r--r--   0        0        0     1747 2023-07-07 20:11:33.426000 better_web3-1.5.2/better_web3/contract/erc20.py
+-rw-r--r--   0        0        0     2876 2023-07-07 20:11:33.364000 better_web3-1.5.2/better_web3/contract/erc721.py
+-rw-r--r--   0        0        0     6201 2023-07-07 12:07:18.259000 better_web3-1.5.2/better_web3/contract/multicall.py
+-rw-r--r--   0        0        0     4059 2023-07-26 11:29:17.505000 better_web3-1.5.2/better_web3/proxy.py
+-rw-r--r--   0        0        0      730 2023-07-17 08:28:26.473000 better_web3-1.5.2/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-17 08:28:28.447000 better_web3-1.5.2/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4132 2023-07-17 08:28:28.496000 better_web3-1.5.2/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.5.2/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     1398 2023-07-11 06:39:33.869000 better_web3-1.5.2/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0     2131 2023-07-17 08:28:26.617000 better_web3-1.5.2/better_web3/utils/eth.py
+-rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.5.2/better_web3/utils/file.py
+-rw-r--r--   0        0        0      663 2023-07-07 20:05:19.087000 better_web3-1.5.2/better_web3/utils/other.py
+-rw-r--r--   0        0        0     3227 2023-07-26 11:29:17.244000 better_web3-1.5.2/better_web3/wallet.py
+-rw-r--r--   0        0        0      412 2023-07-27 14:36:24.313000 better_web3-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      479 2023-07-07 17:47:32.398000 better_web3-1.5.2/README.md
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 better_web3-1.5.2/PKG-INFO
```

### Comparing `better_web3-1.5.1/better_web3/batch_call.py` & `better_web3-1.5.2/better_web3/batch_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,16 @@
 
 
 class Manager:
     def __init__(self, chain: "Chain"):
         self.chain = chain
         self.rpc = chain.rpc
         self.w3 = chain.w3
-        self.slow_w3 = chain.slow_w3
         self.http_session = chain.http_session
         self.timeout = chain.timeout
-        self.slow_timeout = chain.slow_timeout
 
 
 class BatchCallManager(Manager):
 
     def __init__(
             self,
             chain: "Chain",
@@ -115,15 +113,15 @@
         if not payloads:
             return []
 
         batch_size = batch_size or self.batch_request_size
         delay = delay or self.batch_request_delay
 
         for chunk in chunks(payloads, batch_size):
-            response = self.http_session.post(self.rpc, json=chunk, timeout=self.slow_timeout)
+            response = self.http_session.post(self.rpc, json=chunk, timeout=self.timeout)
             results = response.json()
             for payload, response in zip(chunk, process_results(results, raise_exceptions=raise_exceptions)):
                 result = {"payload": payload}
                 if isinstance(response, JSONRPCException):
                     result["exception"] = response
                 else:
                     result["result"] = response
```

### Comparing `better_web3-1.5.1/better_web3/chain.py` & `better_web3-1.5.2/better_web3/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
             multicall_v3_contract_address: ChecksumAddress | str = None,
             # Disperse
             disperse_contract_address: ChecksumAddress | str = None,
             # Batch request
             batch_request_size: int = 10,
             batch_request_delay: int = 1,
             # Tx params
-            gas: int = None,
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
             max_fee_per_gas: Wei | int = None,
             max_priority_fee_per_gas: Wei | int = None,
     ):
         self._rpc = rpc
@@ -84,15 +83,14 @@
 
         self.multicall = Multicall(chain=self, address=multicall_v3_contract_address)
         self.disperse = Disperse(chain=self, address=disperse_contract_address)
 
         self.batch_request = BatchCallManager(
             self, batch_request_size, batch_request_delay)
 
-        self.default_gas = gas
         self.default_gas_price = gas_price
         self.default_max_fee_per_gas = max_fee_per_gas
         self.default_max_priority_fee_per_gas = max_priority_fee_per_gas
 
     def _create_http_provider(self, timeout: int) -> HTTPProvider:
         return HTTPProvider(
             self._rpc,
```

### Comparing `better_web3-1.5.1/better_web3/contract/__pycache__/__init__.cpython-311.pyc` & `better_web3-1.5.2/better_web3/contract/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/__pycache__/_abi.cpython-311.pyc` & `better_web3-1.5.2/better_web3/contract/__pycache__/_abi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/__pycache__/contract.cpython-311.pyc` & `better_web3-1.5.2/better_web3/contract/__pycache__/contract.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/__pycache__/disperse.cpython-311.pyc` & `better_web3-1.5.2/better_web3/contract/__pycache__/disperse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc` & `better_web3-1.5.2/better_web3/contract/__pycache__/erc20.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc` & `better_web3-1.5.2/better_web3/contract/__pycache__/erc721.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-1.5.2/better_web3/contract/__pycache__/multicall.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/abi/disperse.json` & `better_web3-1.5.2/better_web3/contract/abi/disperse.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/abi/erc1155.json` & `better_web3-1.5.2/better_web3/contract/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/abi/erc20.json` & `better_web3-1.5.2/better_web3/contract/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/abi/erc721.json` & `better_web3-1.5.2/better_web3/contract/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/abi/multicall_v3.json` & `better_web3-1.5.2/better_web3/contract/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/contract.py` & `better_web3-1.5.2/better_web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/disperse.py` & `better_web3-1.5.2/better_web3/contract/disperse.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/erc20.py` & `better_web3-1.5.2/better_web3/contract/erc20.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/erc721.py` & `better_web3-1.5.2/better_web3/contract/erc721.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/contract/multicall.py` & `better_web3-1.5.2/better_web3/contract/multicall.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/proxy.py` & `better_web3-1.5.2/better_web3/proxy.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/__init__.py` & `better_web3-1.5.2/better_web3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-1.5.2/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-1.5.2/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/__pycache__/file.cpython-311.pyc` & `better_web3-1.5.2/better_web3/utils/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-1.5.2/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/eth.py` & `better_web3-1.5.2/better_web3/utils/eth.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/file.py` & `better_web3-1.5.2/better_web3/utils/file.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/utils/other.py` & `better_web3-1.5.2/better_web3/utils/other.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/better_web3/wallet.py` & `better_web3-1.5.2/better_web3/wallet.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.5.1/PKG-INFO` & `better_web3-1.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 1.5.1
+Version: 1.5.2
 Summary: Chains, Contracts(Multicall, Disperse, ERC20/ERC721), batch calls and other..
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: web3 (>=6.6.1,<7.0.0)
+Requires-Dist: web3 (>=6.7.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Better Web3.py
 [ [Telegram](https://t.me/cum_insider) ] [ [PyPi](https://pypi.org/project/better-web3) ]
 
 ```bash
 pip install better-web3
```

