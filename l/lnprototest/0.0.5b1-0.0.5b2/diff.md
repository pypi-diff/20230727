# Comparing `tmp/lnprototest-0.0.5b1.tar.gz` & `tmp/lnprototest-0.0.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnprototest-0.0.5b1.tar", max compression
+gzip compressed data, was "lnprototest-0.0.5b2.tar", max compression
```

## Comparing `lnprototest-0.0.5b1.tar` & `lnprototest-0.0.5b2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2418 2023-03-01 18:25:00.167598 lnprototest-0.0.5b1/README.md
--rw-r--r--   0        0        0     3353 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/__init__.py
--rw-r--r--   0        0        0       95 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/backend/__init__.py
--rw-r--r--   0        0        0      554 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/backend/backend.py
--rw-r--r--   0        0        0     6598 2023-07-27 16:48:40.280552 lnprototest-0.0.5b1/lnprototest/backend/bitcoind.py
--rw-r--r--   0        0        0     1114 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/bitfield.py
--rw-r--r--   0        0        0      645 2023-03-01 18:25:00.167598 lnprototest-0.0.5b1/lnprototest/clightning/__init__.py
--rw-r--r--   0        0        0    19098 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/clightning/clightning.py
--rw-r--r--   0        0        0       12 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/clightning/requirements.txt
--rw-r--r--   0        0        0   150826 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/commit_tx.py
--rw-r--r--   0        0        0     6948 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/dummyrunner.py
--rw-r--r--   0        0        0      849 2023-03-01 18:25:00.170931 lnprototest-0.0.5b1/lnprototest/errors.py
--rw-r--r--   0        0        0    24013 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/event.py
--rw-r--r--   0        0        0    31655 2023-06-24 07:36:27.198027 lnprototest-0.0.5b1/lnprototest/funding.py
--rw-r--r--   0        0        0     6133 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/keyset.py
--rwxr-xr-x   0        0        0     1013 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/namespace.py
--rw-r--r--   0        0        0     4619 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/proposals.py
--rw-r--r--   0        0        0    10292 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/runner.py
--rwxr-xr-x   0        0        0     5570 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/signature.py
--rw-r--r--   0        0        0      817 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/stash/__init__.py
--rw-r--r--   0        0        0     9145 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/stash/stash.py
--rw-r--r--   0        0        0     9117 2023-02-27 21:38:00.613217 lnprototest-0.0.5b1/lnprototest/structure.py
--rw-r--r--   0        0        0      480 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/utils/__init__.py
--rw-r--r--   0        0        0     8530 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/utils/bitcoin_utils.py
--rw-r--r--   0        0        0     7954 2023-07-22 16:26:10.243963 lnprototest-0.0.5b1/lnprototest/utils/ln_spec_utils.py
--rw-r--r--   0        0        0     3058 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/utils/utils.py
--rw-r--r--   0        0        0      904 2023-07-27 16:48:32.626862 lnprototest-0.0.5b1/pyproject.toml
--rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 lnprototest-0.0.5b1/PKG-INFO
+-rw-r--r--   0        0        0     2418 2023-03-01 18:25:00.167598 lnprototest-0.0.5b2/README.md
+-rw-r--r--   0        0        0     3353 2023-07-25 13:35:33.787615 lnprototest-0.0.5b2/lnprototest/__init__.py
+-rw-r--r--   0        0        0       95 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/backend/__init__.py
+-rw-r--r--   0        0        0      554 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/backend/backend.py
+-rw-r--r--   0        0        0     6660 2023-07-27 17:12:37.031814 lnprototest-0.0.5b2/lnprototest/backend/bitcoind.py
+-rw-r--r--   0        0        0     1114 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/bitfield.py
+-rw-r--r--   0        0        0      645 2023-03-01 18:25:00.167598 lnprototest-0.0.5b2/lnprototest/clightning/__init__.py
+-rw-r--r--   0        0        0    19098 2023-07-25 13:35:33.787615 lnprototest-0.0.5b2/lnprototest/clightning/clightning.py
+-rw-r--r--   0        0        0       12 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/clightning/requirements.txt
+-rw-r--r--   0        0        0   150826 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/commit_tx.py
+-rw-r--r--   0        0        0     6948 2023-07-25 13:35:33.787615 lnprototest-0.0.5b2/lnprototest/dummyrunner.py
+-rw-r--r--   0        0        0      849 2023-03-01 18:25:00.170931 lnprototest-0.0.5b2/lnprototest/errors.py
+-rw-r--r--   0        0        0    24013 2023-07-25 13:35:33.787615 lnprototest-0.0.5b2/lnprototest/event.py
+-rw-r--r--   0        0        0    31655 2023-06-24 07:36:27.198027 lnprototest-0.0.5b2/lnprototest/funding.py
+-rw-r--r--   0        0        0     6132 2023-07-27 17:12:37.031814 lnprototest-0.0.5b2/lnprototest/keyset.py
+-rwxr-xr-x   0        0        0     1013 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/namespace.py
+-rw-r--r--   0        0        0     4619 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/proposals.py
+-rw-r--r--   0        0        0    10292 2023-07-25 13:35:33.787615 lnprototest-0.0.5b2/lnprototest/runner.py
+-rwxr-xr-x   0        0        0     5570 2023-02-14 10:36:29.511225 lnprototest-0.0.5b2/lnprototest/signature.py
+-rw-r--r--   0        0        0      817 2023-06-24 07:36:27.201361 lnprototest-0.0.5b2/lnprototest/stash/__init__.py
+-rw-r--r--   0        0        0     9145 2023-06-24 07:36:27.201361 lnprototest-0.0.5b2/lnprototest/stash/stash.py
+-rw-r--r--   0        0        0     9117 2023-02-27 21:38:00.613217 lnprototest-0.0.5b2/lnprototest/structure.py
+-rw-r--r--   0        0        0      480 2023-07-25 13:35:33.787615 lnprototest-0.0.5b2/lnprototest/utils/__init__.py
+-rw-r--r--   0        0        0     8530 2023-06-24 07:36:27.201361 lnprototest-0.0.5b2/lnprototest/utils/bitcoin_utils.py
+-rw-r--r--   0        0        0     7954 2023-07-22 16:26:10.243963 lnprototest-0.0.5b2/lnprototest/utils/ln_spec_utils.py
+-rw-r--r--   0        0        0     3058 2023-07-25 13:35:33.787615 lnprototest-0.0.5b2/lnprototest/utils/utils.py
+-rw-r--r--   0        0        0      904 2023-07-27 17:13:09.573148 lnprototest-0.0.5b2/pyproject.toml
+-rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 lnprototest-0.0.5b2/PKG-INFO
```

### Comparing `lnprototest-0.0.5b1/README.md` & `lnprototest-0.0.5b2/README.md`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/__init__.py` & `lnprototest-0.0.5b2/lnprototest/__init__.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/backend/backend.py` & `lnprototest-0.0.5b2/lnprototest/backend/backend.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/backend/bitcoind.py` & `lnprototest-0.0.5b2/lnprototest/backend/bitcoind.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import shutil
 import subprocess
 import logging
 import socket
 
 from contextlib import closing
-from typing import Any, Callable
+from typing import Any, Callable, Optional
 from bitcoin.rpc import RawProxy
 from .backend import Backend
 
 
 class BitcoinProxy:
     """Wrapper for BitcoinProxy to reconnect.
 
@@ -48,15 +48,15 @@
         f.__name__ = name
         return f
 
 
 class Bitcoind(Backend):
     """Starts regtest bitcoind on an ephemeral port, and returns the RPC proxy"""
 
-    def __init__(self, basedir: str, with_wallet: bool = True):
+    def __init__(self, basedir: str, with_wallet: Optional[str] = None):
         self.with_wallet = with_wallet
         self.rpc = None
         self.proc = None
         self.base_dir = basedir
         logging.debug(f"Base dir is {basedir}")
         self.bitcoin_dir = os.path.join(basedir, "bitcoind")
         self.bitcoin_conf = os.path.join(self.bitcoin_dir, "bitcoin.conf")
@@ -116,16 +116,17 @@
 
         self.btc_version = self.rpc.getnetworkinfo()["version"]
         assert self.btc_version is not None
         logging.debug("Bitcoin Core version {}".format(self.btc_version))
         if self.btc_version >= 210000:
             # Maintains the compatibility between wallet
             # different ln implementation can use the main wallet (?)
-            if self.with_wallet:
-                self.rpc.createwallet("main")  # Automatically loads
+            self.rpc.createwallet(
+                "main" if self.with_wallet is None else self.with_wallet
+            )  # Automatically loads
 
     def __is__bitcoind_ready(self) -> bool:
         """Check if bitcoind is ready during the execution"""
         if self.proc is None:
             # Sanity check
             raise ValueError("bitcoind not initialized")
```

### Comparing `lnprototest-0.0.5b1/lnprototest/bitfield.py` & `lnprototest-0.0.5b2/lnprototest/bitfield.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/clightning/__init__.py` & `lnprototest-0.0.5b2/lnprototest/clightning/__init__.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/clightning/clightning.py` & `lnprototest-0.0.5b2/lnprototest/clightning/clightning.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/commit_tx.py` & `lnprototest-0.0.5b2/lnprototest/commit_tx.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/dummyrunner.py` & `lnprototest-0.0.5b2/lnprototest/dummyrunner.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/errors.py` & `lnprototest-0.0.5b2/lnprototest/errors.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/event.py` & `lnprototest-0.0.5b2/lnprototest/event.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/funding.py` & `lnprototest-0.0.5b2/lnprototest/funding.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/keyset.py` & `lnprototest-0.0.5b2/lnprototest/keyset.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         self,
         revocation_base_secret: str,
         payment_base_secret: str,
         htlc_base_secret: str,
         delayed_payment_base_secret: str,
         shachain_seed: str,
     ):
-
         from .utils import privkey_expand, check_hex
 
         self.revocation_base_secret = privkey_expand(revocation_base_secret)
         self.payment_base_secret = privkey_expand(payment_base_secret)
         self.htlc_base_secret = privkey_expand(htlc_base_secret)
         self.delayed_payment_base_secret = privkey_expand(delayed_payment_base_secret)
         self.shachain_seed = bytes.fromhex(check_hex(shachain_seed, 64))
```

### Comparing `lnprototest-0.0.5b1/lnprototest/namespace.py` & `lnprototest-0.0.5b2/lnprototest/namespace.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/proposals.py` & `lnprototest-0.0.5b2/lnprototest/proposals.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/runner.py` & `lnprototest-0.0.5b2/lnprototest/runner.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/signature.py` & `lnprototest-0.0.5b2/lnprototest/signature.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/stash/__init__.py` & `lnprototest-0.0.5b2/lnprototest/stash/__init__.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/stash/stash.py` & `lnprototest-0.0.5b2/lnprototest/stash/stash.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/structure.py` & `lnprototest-0.0.5b2/lnprototest/structure.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/utils/bitcoin_utils.py` & `lnprototest-0.0.5b2/lnprototest/utils/bitcoin_utils.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/utils/ln_spec_utils.py` & `lnprototest-0.0.5b2/lnprototest/utils/ln_spec_utils.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/lnprototest/utils/utils.py` & `lnprototest-0.0.5b2/lnprototest/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.5b1/pyproject.toml` & `lnprototest-0.0.5b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lnprototest"
-version = "0.0.5-beta.1"
+version = "0.0.5-beta.2"
 description = "Spec protocol tests for lightning network implementations"
 authors = ["Rusty Russell <rusty@blockstream.com>", "Vincenzo Palazzo <vincenzopalazzodev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `lnprototest-0.0.5b1/PKG-INFO` & `lnprototest-0.0.5b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnprototest
-Version: 0.0.5b1
+Version: 0.0.5b2
 Summary: Spec protocol tests for lightning network implementations
 License: MIT
 Author: Rusty Russell
 Author-email: rusty@blockstream.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lnprototest Version: 0.0.5b1 Summary: Spec protocol
+Metadata-Version: 2.1 Name: lnprototest Version: 0.0.5b2 Summary: Spec protocol
 tests for lightning network implementations License: MIT Author: Rusty Russell
 Author-email: rusty@blockstream.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: crc32c (>=2.2.post0,<3.0)
```

