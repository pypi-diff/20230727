# Comparing `tmp/lnprototest-0.0.4.tar.gz` & `tmp/lnprototest-0.0.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnprototest-0.0.4.tar", max compression
+gzip compressed data, was "lnprototest-0.0.5b1.tar", max compression
```

## Comparing `lnprototest-0.0.4.tar` & `lnprototest-0.0.5b1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2418 2023-03-01 18:25:00.167598 lnprototest-0.0.4/README.md
--rw-r--r--   0        0        0     3353 2023-06-01 22:01:01.582905 lnprototest-0.0.4/lnprototest/__init__.py
--rw-r--r--   0        0        0       95 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/backend/__init__.py
--rw-r--r--   0        0        0      554 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/backend/backend.py
--rw-r--r--   0        0        0     6496 2023-03-01 18:25:00.167598 lnprototest-0.0.4/lnprototest/backend/bitcoind.py
--rw-r--r--   0        0        0     1114 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/bitfield.py
--rw-r--r--   0        0        0      645 2023-03-01 18:25:00.167598 lnprototest-0.0.4/lnprototest/clightning/__init__.py
--rw-r--r--   0        0        0    19098 2023-06-01 23:07:19.594928 lnprototest-0.0.4/lnprototest/clightning/clightning.py
--rw-r--r--   0        0        0       12 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/clightning/requirements.txt
--rw-r--r--   0        0        0   150826 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/commit_tx.py
--rw-r--r--   0        0        0     6948 2023-06-01 22:43:33.042532 lnprototest-0.0.4/lnprototest/dummyrunner.py
--rw-r--r--   0        0        0      849 2023-03-01 18:25:00.170931 lnprototest-0.0.4/lnprototest/errors.py
--rw-r--r--   0        0        0    23405 2023-06-03 15:19:03.207606 lnprototest-0.0.4/lnprototest/event.py
--rw-r--r--   0        0        0    31655 2023-06-01 22:00:10.587565 lnprototest-0.0.4/lnprototest/funding.py
--rw-r--r--   0        0        0     6133 2023-06-01 22:35:32.610636 lnprototest-0.0.4/lnprototest/keyset.py
--rwxr-xr-x   0        0        0     1013 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/namespace.py
--rw-r--r--   0        0        0     4619 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/proposals.py
--rw-r--r--   0        0        0     9918 2023-03-01 18:25:00.170931 lnprototest-0.0.4/lnprototest/runner.py
--rwxr-xr-x   0        0        0     5570 2023-02-14 10:36:29.511225 lnprototest-0.0.4/lnprototest/signature.py
--rw-r--r--   0        0        0      817 2023-06-01 20:30:01.524336 lnprototest-0.0.4/lnprototest/stash/__init__.py
--rw-r--r--   0        0        0     9145 2023-06-03 15:25:28.179410 lnprototest-0.0.4/lnprototest/stash/stash.py
--rw-r--r--   0        0        0     9117 2023-02-27 21:38:00.613217 lnprototest-0.0.4/lnprototest/structure.py
--rw-r--r--   0        0        0      480 2023-06-01 22:36:58.710620 lnprototest-0.0.4/lnprototest/utils/__init__.py
--rw-r--r--   0        0        0     8530 2023-06-01 21:57:15.467339 lnprototest-0.0.4/lnprototest/utils/bitcoin_utils.py
--rw-r--r--   0        0        0     8585 2023-06-03 15:25:28.156076 lnprototest-0.0.4/lnprototest/utils/ln_spec_utils.py
--rw-r--r--   0        0        0     3058 2023-06-01 22:46:52.836969 lnprototest-0.0.4/lnprototest/utils/utils.py
--rw-r--r--   0        0        0      896 2023-06-03 15:40:36.775497 lnprototest-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 lnprototest-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2418 2023-03-01 18:25:00.167598 lnprototest-0.0.5b1/README.md
+-rw-r--r--   0        0        0     3353 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/__init__.py
+-rw-r--r--   0        0        0       95 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/backend/__init__.py
+-rw-r--r--   0        0        0      554 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/backend/backend.py
+-rw-r--r--   0        0        0     6598 2023-07-27 16:48:40.280552 lnprototest-0.0.5b1/lnprototest/backend/bitcoind.py
+-rw-r--r--   0        0        0     1114 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/bitfield.py
+-rw-r--r--   0        0        0      645 2023-03-01 18:25:00.167598 lnprototest-0.0.5b1/lnprototest/clightning/__init__.py
+-rw-r--r--   0        0        0    19098 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/clightning/clightning.py
+-rw-r--r--   0        0        0       12 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/clightning/requirements.txt
+-rw-r--r--   0        0        0   150826 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/commit_tx.py
+-rw-r--r--   0        0        0     6948 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/dummyrunner.py
+-rw-r--r--   0        0        0      849 2023-03-01 18:25:00.170931 lnprototest-0.0.5b1/lnprototest/errors.py
+-rw-r--r--   0        0        0    24013 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/event.py
+-rw-r--r--   0        0        0    31655 2023-06-24 07:36:27.198027 lnprototest-0.0.5b1/lnprototest/funding.py
+-rw-r--r--   0        0        0     6133 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/keyset.py
+-rwxr-xr-x   0        0        0     1013 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/namespace.py
+-rw-r--r--   0        0        0     4619 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/proposals.py
+-rw-r--r--   0        0        0    10292 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/runner.py
+-rwxr-xr-x   0        0        0     5570 2023-02-14 10:36:29.511225 lnprototest-0.0.5b1/lnprototest/signature.py
+-rw-r--r--   0        0        0      817 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/stash/__init__.py
+-rw-r--r--   0        0        0     9145 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/stash/stash.py
+-rw-r--r--   0        0        0     9117 2023-02-27 21:38:00.613217 lnprototest-0.0.5b1/lnprototest/structure.py
+-rw-r--r--   0        0        0      480 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/utils/__init__.py
+-rw-r--r--   0        0        0     8530 2023-06-24 07:36:27.201361 lnprototest-0.0.5b1/lnprototest/utils/bitcoin_utils.py
+-rw-r--r--   0        0        0     7954 2023-07-22 16:26:10.243963 lnprototest-0.0.5b1/lnprototest/utils/ln_spec_utils.py
+-rw-r--r--   0        0        0     3058 2023-07-25 13:35:33.787615 lnprototest-0.0.5b1/lnprototest/utils/utils.py
+-rw-r--r--   0        0        0      904 2023-07-27 16:48:32.626862 lnprototest-0.0.5b1/pyproject.toml
+-rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 lnprototest-0.0.5b1/PKG-INFO
```

### Comparing `lnprototest-0.0.4/README.md` & `lnprototest-0.0.5b1/README.md`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/__init__.py` & `lnprototest-0.0.5b1/lnprototest/__init__.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/backend/backend.py` & `lnprototest-0.0.5b1/lnprototest/backend/backend.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/backend/bitcoind.py` & `lnprototest-0.0.5b1/lnprototest/backend/bitcoind.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         f.__name__ = name
         return f
 
 
 class Bitcoind(Backend):
     """Starts regtest bitcoind on an ephemeral port, and returns the RPC proxy"""
 
-    def __init__(self, basedir: str):
+    def __init__(self, basedir: str, with_wallet: bool = True):
+        self.with_wallet = with_wallet
         self.rpc = None
         self.proc = None
         self.base_dir = basedir
         logging.debug(f"Base dir is {basedir}")
         self.bitcoin_dir = os.path.join(basedir, "bitcoind")
         self.bitcoin_conf = os.path.join(self.bitcoin_dir, "bitcoin.conf")
         self.cmd_line = [
@@ -115,15 +116,16 @@
 
         self.btc_version = self.rpc.getnetworkinfo()["version"]
         assert self.btc_version is not None
         logging.debug("Bitcoin Core version {}".format(self.btc_version))
         if self.btc_version >= 210000:
             # Maintains the compatibility between wallet
             # different ln implementation can use the main wallet (?)
-            self.rpc.createwallet("main")  # Automatically loads
+            if self.with_wallet:
+                self.rpc.createwallet("main")  # Automatically loads
 
     def __is__bitcoind_ready(self) -> bool:
         """Check if bitcoind is ready during the execution"""
         if self.proc is None:
             # Sanity check
             raise ValueError("bitcoind not initialized")
```

### Comparing `lnprototest-0.0.4/lnprototest/bitfield.py` & `lnprototest-0.0.5b1/lnprototest/bitfield.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/clightning/__init__.py` & `lnprototest-0.0.5b1/lnprototest/clightning/__init__.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/clightning/clightning.py` & `lnprototest-0.0.5b1/lnprototest/clightning/clightning.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/commit_tx.py` & `lnprototest-0.0.5b1/lnprototest/commit_tx.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/dummyrunner.py` & `lnprototest-0.0.5b1/lnprototest/dummyrunner.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/errors.py` & `lnprototest-0.0.5b1/lnprototest/errors.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/event.py` & `lnprototest-0.0.5b1/lnprototest/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,18 @@
         return True
 
 
 class Block(Event):
     """Generate a block, at blockheight, with optional txs."""
 
     def __init__(
-        self, blockheight: int, number: int = 1, txs: List[ResolvableStr] = []
+        self,
+        blockheight: int,
+        number: Union[int, Callable] = 1,
+        txs: List[ResolvableStr] = [],
     ):
         super().__init__()
         self.blockheight = blockheight
         self.number = number
         self.txs = txs
 
     def action(self, runner: "Runner") -> bool:
@@ -395,14 +398,17 @@
                 ),
             )
 
         # Throw away blocks we're replacing.
         if runner.getblockheight() >= self.blockheight:
             runner.trim_blocks(self.blockheight - 1)
 
+        if isinstance(self.number, Callable):
+            self.number = self.resolve_arg(None, runner, self.number)
+
         # Add new one
         runner.add_blocks(
             self, [self.resolve_arg("tx", runner, tx) for tx in self.txs], self.number
         )
         assert runner.getblockheight() == self.blockheight - 1 + self.number
         return True
 
@@ -532,14 +538,24 @@
         super().__init__(connprivkey)
 
     def action(self, runner: "Runner") -> bool:
         super().action(runner)
         error = runner.check_error(self, self.find_conn(runner))
         if error is None:
             raise EventError(self, "No error found")
+        if runner._is_dummy():
+            return True
+        error = bytes.fromhex(error)
+        msg = Message.read(namespace(), io.BytesIO(error))
+        logging.info(f"message received {msg.messagetype.name}, hex {error.hex()}")
+        if msg.messagetype.name not in "error":
+            raise EventError(
+                self,
+                f"not error found but received `{msg.messagetype.name}` with hex: `{error.hex()}`",
+            )
         return True
 
 
 class ExpectDisconnect(PerConnEvent):
     """This is considerer an hack, because the protocol
     is not specifing what fail the connection means, so in
     some case a node close the connection without any message
```

### Comparing `lnprototest-0.0.4/lnprototest/funding.py` & `lnprototest-0.0.5b1/lnprototest/funding.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/keyset.py` & `lnprototest-0.0.5b1/lnprototest/keyset.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/namespace.py` & `lnprototest-0.0.5b1/lnprototest/namespace.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/proposals.py` & `lnprototest-0.0.5b1/lnprototest/proposals.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/runner.py` & `lnprototest-0.0.5b1/lnprototest/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import shutil
 import tempfile
 
 import coincurve
 import functools
 
+from .bitfield import bitfield
 from .errors import SpecFileError
 from .structure import Sequence
 from .event import Event, MustNotMsg, ExpectMsg
 from .utils import privkey_expand
 from .keyset import KeySet
 from abc import ABC, abstractmethod
 from typing import Dict, Optional, List, Union, Any, Callable
@@ -116,14 +117,27 @@
         return self.stash[stashname]
 
     def teardown(self):
         """The Teardown method is called at the end of the test,
         and it is used to clean up the root dir where the tests are run."""
         shutil.rmtree(self.directory)
 
+    def runner_features(
+        self,
+        additional_features: Optional[List[int]] = None,
+        globals: bool = False,
+    ) -> str:
+        """
+        Provide the features required by the node.
+        """
+        if additional_features is None:
+            return ""
+        else:
+            return bitfield(*additional_features)
+
     @abstractmethod
     def is_running(self) -> bool:
         """Return a boolean value that tells whether the runner is running
         or not.
         Is leave up to the runner implementation to keep the runner state"""
         pass
```

### Comparing `lnprototest-0.0.4/lnprototest/signature.py` & `lnprototest-0.0.5b1/lnprototest/signature.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/stash/__init__.py` & `lnprototest-0.0.5b1/lnprototest/stash/__init__.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/stash/stash.py` & `lnprototest-0.0.5b1/lnprototest/stash/stash.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/structure.py` & `lnprototest-0.0.5b1/lnprototest/structure.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/utils/bitcoin_utils.py` & `lnprototest-0.0.5b1/lnprototest/utils/bitcoin_utils.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/lnprototest/utils/ln_spec_utils.py` & `lnprototest-0.0.5b1/lnprototest/utils/ln_spec_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,39 +45,43 @@
         return f"{block_height}x{tx_idx}x{tx_output}"
 
 
 def connect_to_node_helper(
     runner: "Runner",
     tx_spendable: str,
     conn_privkey: str = "02",
-    global_features: Optional[str] = None,
-    features: Optional[str] = None,
+    global_features: Optional[List[int]] = None,
+    features: Optional[List[int]] = None,
 ) -> List["Event"]:
     """Helper function to make a connection with the node"""
     from lnprototest.utils.bitcoin_utils import tx_spendable
-    from lnprototest.stash import stash_field_from_event
     from lnprototest import (
         Connect,
         Block,
         ExpectMsg,
         Msg,
     )
 
     return [
         Block(blockheight=102, txs=[tx_spendable]),
         Connect(connprivkey=conn_privkey),
         ExpectMsg("init"),
         Msg(
             "init",
-            globalfeatures=stash_field_from_event("init", dummy_val="")
+            globalfeatures=runner.runner_features(globals=True)
             if global_features is None
-            else global_features,
-            features=stash_field_from_event("init", dummy_val="")
+            else (
+                runner.runner_features(
+                    global_features,
+                    globals=True,
+                )
+            ),
+            features=runner.runner_features()
             if features is None
-            else features,
+            else (runner.runner_features(features)),
         ),
     ]
 
 
 def open_and_announce_channel_helper(
     runner: "Runner", conn_privkey: str = "02", opts: dict = {}
 ) -> List["Event"]:
@@ -109,14 +113,15 @@
         funding,
         sent,
         commitsig_to_recv,
         channel_id,
         commitsig_to_send,
         funding_txid,
         funding_tx,
+        stash_field_from_event,
     )
 
     # Make up a channel between nodes 02 and 03, using bitcoin privkeys 10 and 20
     local_keyset = gen_random_keyset()
     local_funding_privkey = "20"
     if "block_height" in opts:
         block_height = opts["block_height"]
@@ -153,15 +158,15 @@
             "accept_channel",
             funding_pubkey=remote_funding_pubkey(),
             revocation_basepoint=remote_revocation_basepoint(),
             payment_basepoint=remote_payment_basepoint(),
             delayed_payment_basepoint=remote_delayed_payment_basepoint(),
             htlc_basepoint=remote_htlc_basepoint(),
             first_per_commitment_point=remote_per_commitment_point(0),
-            minimum_depth=3,
+            minimum_depth=stash_field_from_event("accept_channel", dummy_val=3),
             channel_reserve_satoshis=9998,
         ),
         # Create and stash Funding object and FundingTx
         CreateFunding(
             *utxo(0),
             local_node_privkey="02",
             local_funding_privkey=local_funding_privkey,
@@ -189,38 +194,31 @@
             funding_output_index=0,
             signature=commitsig_to_send(),
         ),
         ExpectMsg(
             "funding_signed", channel_id=channel_id(), signature=commitsig_to_recv()
         ),
         # Mine it and get it deep enough to confirm channel.
-        Block(blockheight=103, number=3, txs=[funding_tx()]),
+        Block(
+            blockheight=103,
+            number=stash_field_from_event(
+                "accept_channel", field_name="minimum_depth", dummy_val=3
+            ),
+            txs=[funding_tx()],
+        ),
         ExpectMsg(
             "channel_ready",
             channel_id=channel_id(),
             second_per_commitment_point=remote_per_commitment_point(1),
         ),
         Msg(
             "channel_ready",
             channel_id=channel_id(),
             second_per_commitment_point=local_keyset.per_commit_point(1),
         ),
         # wait confirmations
         Block(blockheight=103, number=6),
-        # FIXME: implement all the utils function for the announcement_signatures
-        ExpectMsg(
-            "announcement_signatures",
-            channel_id=channel_id(),
-            short_channel_id=short_channel_id,
-            # TODO: How build signatures without hard coding it here?
-            node_signature="5ffb05bfb1ef2941cd26e02eea9bfcd6862a08dcfd58473cd1e7da879c2127d6650159c731ae07cd07ff00f4fe7d344aef7997384465f34d7c57add4795a7b09",
-            bitcoin_signature="138c93afb2013c39f959e70a163c3d6d8128cf72f8ae143f87b9d1fd6bb0ad30321116b9c58d69fca9fb33c214f681b664e53d5640abc2fdb972dc62a5571053",
-        ),
-        Msg(
-            "announcement_signatures",
-            channel_id=channel_id(),
-            short_channel_id=short_channel_id,
-            # TODO: How build signatures without hard coding it here?
-            node_signature="5ffb05bfb1ef2941cd26e02eea9bfcd6862a08dcfd58473cd1e7da879c2127d6650159c731ae07cd07ff00f4fe7d344aef7997384465f34d7c57add4795a7b09",
-            bitcoin_signature="138c93afb2013c39f959e70a163c3d6d8128cf72f8ae143f87b9d1fd6bb0ad30321116b9c58d69fca9fb33c214f681b664e53d5640abc2fdb972dc62a5571053",
-        ),
+        # BOLT 2:
+        #
+        # Once both nodes have exchanged channel_ready (and optionally announcement_signatures),
+        # the channel can be used to make payments via Hashed Time Locked Contracts.
     ]
```

### Comparing `lnprototest-0.0.4/lnprototest/utils/utils.py` & `lnprototest-0.0.5b1/lnprototest/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lnprototest-0.0.4/pyproject.toml` & `lnprototest-0.0.5b1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lnprototest"
-version = "0.0.4"
+version = "0.0.5-beta.1"
 description = "Spec protocol tests for lightning network implementations"
 authors = ["Rusty Russell <rusty@blockstream.com>", "Vincenzo Palazzo <vincenzopalazzodev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -13,15 +13,15 @@
 pyln-bolt1 = "^1.0.222"
 pyln-client = "^0.12.0"
 pyln-testing = "^0.12.0"
 crc32c = "^2.2.post0"
 # We accidentally published version 1.0.186 instead of 1.0.2.186. That
 # version is now yanked by caches remain, so this is a temporary fix.
 pyln-bolt7 = "^1.0.246"
-pyln-proto = "^0.12.0"
+pyln-proto = "^23.05.2"
 python-bitcoinlib = "^0.11.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^22.1.0"
 flake8 = "^4.0.1"
 pytest-xdist = "^3.1.0"
```

### Comparing `lnprototest-0.0.4/PKG-INFO` & `lnprototest-0.0.5b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnprototest
-Version: 0.0.4
+Version: 0.0.5b1
 Summary: Spec protocol tests for lightning network implementations
 License: MIT
 Author: Rusty Russell
 Author-email: rusty@blockstream.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: crc32c (>=2.2.post0,<3.0)
 Requires-Dist: pyln-bolt1 (>=1.0.222,<2.0.0)
 Requires-Dist: pyln-bolt2 (>=1.0.222,<2.0.0)
 Requires-Dist: pyln-bolt4 (>=1.0.222,<2.0.0)
 Requires-Dist: pyln-bolt7 (>=1.0.246,<2.0.0)
 Requires-Dist: pyln-client (>=0.12.0,<0.13.0)
-Requires-Dist: pyln-proto (>=0.12.0,<0.13.0)
+Requires-Dist: pyln-proto (>=23.05.2,<24.0.0)
 Requires-Dist: pyln-testing (>=0.12.0,<0.13.0)
 Requires-Dist: python-bitcoinlib (>=0.11.2,<0.12.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>lnprototest</h1>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: lnprototest Version: 0.0.4 Summary: Spec protocol
+Metadata-Version: 2.1 Name: lnprototest Version: 0.0.5b1 Summary: Spec protocol
 tests for lightning network implementations License: MIT Author: Rusty Russell
 Author-email: rusty@blockstream.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: crc32c (>=2.2.post0,<3.0)
 Requires-Dist: pyln-bolt1 (>=1.0.222,<2.0.0) Requires-Dist: pyln-bolt2
 (>=1.0.222,<2.0.0) Requires-Dist: pyln-bolt4 (>=1.0.222,<2.0.0) Requires-Dist:
 pyln-bolt7 (>=1.0.246,<2.0.0) Requires-Dist: pyln-client (>=0.12.0,<0.13.0)
-Requires-Dist: pyln-proto (>=0.12.0,<0.13.0) Requires-Dist: pyln-testing
+Requires-Dist: pyln-proto (>=23.05.2,<24.0.0) Requires-Dist: pyln-testing
 (>=0.12.0,<0.13.0) Requires-Dist: python-bitcoinlib (>=0.11.2,<0.12.0)
 Description-Content-Type: text/markdown
                            ****** lnprototest ******
                 a Testsuite for the Lightning Network Protocol
                            *** Project_Homepage ***
  [GitHub_Workflow_Status_(branch)] [https://img.shields.io/badge/doc-hacking-
                            orange?style=flat-square]
```

