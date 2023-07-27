# Comparing `tmp/multisig_ci-0.6.4.tar.gz` & `tmp/multisig_ci-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.6.4.tar", max compression
+gzip compressed data, was "multisig_ci-0.6.5.tar", max compression
```

## Comparing `multisig_ci-0.6.4.tar` & `multisig_ci-0.6.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/LICENSE
--rw-r--r--   0        0        0        0 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/__main__.py
--rw-r--r--   0        0        0     7414 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      508 2023-07-27 03:31:54.130489 multisig_ci-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-27 04:05:44.597463 multisig_ci-0.6.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-27 04:05:44.597463 multisig_ci-0.6.5/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     5967 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      508 2023-07-27 04:05:44.601463 multisig_ci-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 multisig_ci-0.6.5/PKG-INFO
```

### Comparing `multisig_ci-0.6.4/LICENSE` & `multisig_ci-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/multisig_ci/__main__.py` & `multisig_ci-0.6.5/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/multisig_ci/ci_override.py` & `multisig_ci-0.6.5/multisig_ci/ci_override.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,74 +14,47 @@
 # that it writes a file with the nonce. This is used to later tag
 # the pull request with a label matching the nonce
 
 DELEGATE_ADDRESS = os.environ.get("DELEGATE_ADDRESS")
 home_directory = os.environ.get("HOME")
 
 gnosis_frontend_urls = {
-    'gnosis': {
-        1: 'https://app.safe.global/eth:{0}/transactions/queue',
-        4: 'https://app.safe.global/rin:{0}/transactions/queue',
-        5: 'https://app.safe.global/gor:{0}/transactions/queue',
-        10: 'https://app.safe.global/oeth:{0}/transactions/queue',
-        56: 'https://app.safe.global/bsc:{0}/transactions/queue',
-        100: 'https://app.safe.global/xdai:{0}/transactions/queue',
-        137: 'https://app.safe.global/matic:{0}/transactions/queue',
-        250: 'https://safe.fantom.network/ftm:{0}/transactions/queue',
-        42161: 'https://app.safe.global/arb1:{0}/transactions/queue'
-    },
-    'yearn': {
-        1: 'http://mainnet.gnosis.yearn.tools/eth:{0}/transactions/queue',
-        4: 'http://mainnet.gnosis.yearn.tools/rin:{0}/transactions/queue',
-        56: 'http://mainnet.gnosis.yearn.tools/bsc:{0}/transactions/queue',
-        100: 'http://mainnet.gnosis.yearn.tools/xdai:{0}/transactions/queue',
-        137: 'http://mainnet.gnosis.yearn.tools/matic:{0}/transactions/queue',
-        42161: 'http://mainnet.gnosis.yearn.tools/arb1:{0}/transactions/queue'
-    }
+    1: 'https://app.safe.global/eth:{0}/transactions/queue',
+    4: 'https://app.safe.global/rin:{0}/transactions/queue',
+    5: 'https://app.safe.global/gor:{0}/transactions/queue',
+    10: 'https://app.safe.global/oeth:{0}/transactions/queue',
+    56: 'https://app.safe.global/bsc:{0}/transactions/queue',
+    100: 'https://app.safe.global/xdai:{0}/transactions/queue',
+    137: 'https://app.safe.global/matic:{0}/transactions/queue',
+    250: 'https://safe.fantom.network/ftm:{0}/transactions/queue',
+    42161: 'https://app.safe.global/arb1:{0}/transactions/queue'
 }
 
 class DelegateSafe(ApeSafe):
     def __init__(self, address, base_url=None, multisend=None):
         """
         Create an ApeSafe from an address or a ENS name and use a default connection.
         """
         multisends[10] = "0x998739BFdAAdde7C933B942a68053933098f9EDa"
-        backend_urls = {
-            'gnosis': self.transaction_service.URLS_BY_NETWORK,
-            'yearn': {1: 'https://safe-transaction.mainnet.gnosis.yearn.tools/'}
-        }
-
-        # default to gnosis if we don't have a yearn version
-        if network.chain.id in backend_urls["gnosis"]:
-            if network.chain.id not in backend_urls[self.backend_type]:
-                backend_url_from_config = backend_urls["gnosis"][network.chain.id]
-                self.frontend_url = ["gnosis"][network.chain.id]
-            else:
-                backend_url_from_config = backend_urls[self.backend_type][network.chain.id]
-                self.frontend_url = gnosis_frontend_urls[self.backend_type][network.chain.id]
+
+        if network.chain.id in gnosis_frontend_urls:
+            self.frontend_url = gnosis_frontend_urls[network.chain.id]
         else:
-            backend_url_from_config = backend_urls["gnosis"][1]
-            self.frontend_url = gnosis_frontend_urls["gnosis"][1]
+            self.frontend_url = gnosis_frontend_urls[1]
 
-        self.base_url = base_url or backend_url_from_config
         super().__init__(address, base_url=self.base_url, multisend=multisend)
 
     @property
     def is_ci(self):
         return os.environ.get("CI", "").lower() == "true"
 
     @property
     def is_send(self):
         return os.environ.get("GITHUB_ACTION_SEND", "").lower() == "true"
 
-    @property
-    def backend_type(self):
-        backend_from_env = os.environ.get("BE", "").lower()
-        return backend_from_env if backend_from_env != "" else "gnosis"
-
     def post_transaction(self, safe_tx: SafeTx):
         super().post_transaction(safe_tx)
 
         if self.is_ci and self.is_send:
             if "{1}" in self.frontend_url:
                 formatted_frontend_url = self.frontend_url.format(self.address, safe_tx.safe_tx_hash.hex())
             else:
```

### Comparing `multisig_ci-0.6.4/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.6.5/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/multisig_ci/run_brownie.py` & `multisig_ci-0.6.5/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/multisig_ci/safes.py` & `multisig_ci-0.6.5/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/multisig_ci/sign.py` & `multisig_ci-0.6.5/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/multisig_ci/telegram.py` & `multisig_ci-0.6.5/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/multisig_ci/test_telegram.sh` & `multisig_ci-0.6.5/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.6.4/PKG-INFO` & `multisig_ci-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.6.4
+Version: 0.6.5
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

