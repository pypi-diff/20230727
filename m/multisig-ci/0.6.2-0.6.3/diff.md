# Comparing `tmp/multisig_ci-0.6.2.tar.gz` & `tmp/multisig_ci-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.6.2.tar", max compression
+gzip compressed data, was "multisig_ci-0.6.3.tar", max compression
```

## Comparing `multisig_ci-0.6.2.tar` & `multisig_ci-0.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/LICENSE
--rw-r--r--   0        0        0        0 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/__main__.py
--rw-r--r--   0        0        0     8308 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      508 2023-07-26 08:17:48.181254 multisig_ci-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     7435 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-27 03:14:43.870093 multisig_ci-0.6.3/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      508 2023-07-27 03:14:43.874093 multisig_ci-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.3/PKG-INFO
```

### Comparing `multisig_ci-0.6.2/LICENSE` & `multisig_ci-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/multisig_ci/__main__.py` & `multisig_ci-0.6.3/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/multisig_ci/ci_override.py` & `multisig_ci-0.6.3/multisig_ci/ci_override.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,42 +35,22 @@
         56: 'http://mainnet.gnosis.yearn.tools/bsc:{0}/transactions/queue',
         100: 'http://mainnet.gnosis.yearn.tools/xdai:{0}/transactions/queue',
         137: 'http://mainnet.gnosis.yearn.tools/matic:{0}/transactions/queue',
         42161: 'http://mainnet.gnosis.yearn.tools/arb1:{0}/transactions/queue'
     }
 }
 
-patched_transaction_service_urls = {
-    1: 'https://safe-transaction-mainnet.safe.global',
-    5: 'https://safe-transaction-goerli.safe.global',
-    10: 'https://safe-transaction-optimism.safe.global',
-    56: 'https://safe-transaction-bsc.safe.global',
-    100: 'https://safe-transaction-gnosis-chain.safe.global',
-    137: 'https://safe-transaction-polygon.safe.global',
-    246: 'https://safe-transaction-ewc.safe.global',
-    250: 'https://safe-txservice.fantom.network',
-    288: 'https://safe-transaction.mainnet.boba.network',
-    42161: 'https://safe-transaction-arbitrum.safe.global',
-    43114: 'https://safe-transaction-avalanche.safe.global',
-    73799: 'https://safe-transaction-volta.safe.global',
-    1313161554: 'https://safe-transaction-aurora.safe.global',
-}
-
 class DelegateSafe(ApeSafe):
     def __init__(self, address, base_url=None, multisend=None):
         """
         Create an ApeSafe from an address or a ENS name and use a default connection.
         """
-        
-        for n, url in patched_transaction_service_urls.items():
-            transaction_service[n] = url
-
         multisends[10] = "0x998739BFdAAdde7C933B942a68053933098f9EDa"
         backend_urls = {
-            'gnosis': transaction_service,
+            'gnosis': self.transaction_service.URLS_BY_NETWORK,
             'yearn': {1: 'https://safe-transaction.mainnet.gnosis.yearn.tools/'}
         }
 
         # default to gnosis if we don't have a yearn version
         if network.chain.id in backend_urls["gnosis"]:
             if network.chain.id not in backend_urls[self.backend_type]:
                 backend_url_from_config = backend_urls["gnosis"][network.chain.id]
```

### Comparing `multisig_ci-0.6.2/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.6.3/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/multisig_ci/run_brownie.py` & `multisig_ci-0.6.3/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/multisig_ci/safes.py` & `multisig_ci-0.6.3/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/multisig_ci/sign.py` & `multisig_ci-0.6.3/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/multisig_ci/telegram.py` & `multisig_ci-0.6.3/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/multisig_ci/test_telegram.sh` & `multisig_ci-0.6.3/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.2/PKG-INFO` & `multisig_ci-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.6.2
+Version: 0.6.3
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

