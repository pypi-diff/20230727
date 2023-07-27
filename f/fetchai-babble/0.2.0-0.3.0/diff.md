# Comparing `tmp/fetchai_babble-0.2.0.tar.gz` & `tmp/fetchai_babble-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchai_babble-0.2.0.tar", max compression
+gzip compressed data, was "fetchai_babble-0.3.0.tar", max compression
```

## Comparing `fetchai_babble-0.2.0.tar` & `fetchai_babble-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-03-14 15:29:41.621719 fetchai_babble-0.2.0/LICENSE
--rw-r--r--   0        0        0      730 2023-01-30 14:03:36.544062 fetchai_babble-0.2.0/README.md
--rw-r--r--   0        0        0      616 2023-04-27 07:56:55.315343 fetchai_babble-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-02-28 15:03:09.430563 fetchai_babble-0.2.0/src/babble/__init__.py
--rw-r--r--   0        0        0     1594 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/auth.py
--rw-r--r--   0        0        0     5925 2023-04-27 07:56:38.515274 fetchai_babble-0.2.0/src/babble/client.py
--rw-r--r--   0        0        0      247 2023-04-27 07:56:38.515274 fetchai_babble-0.2.0/src/babble/config.py
--rw-r--r--   0        0        0       31 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/__init__.py
--rw-r--r--   0        0        0       90 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/exceptions.py
--rw-r--r--   0        0        0      272 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/hashfuncs.py
--rw-r--r--   0        0        0     2911 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/crypto/identity.py
--rw-r--r--   0        0        0      457 2023-01-30 14:03:36.548062 fetchai_babble-0.2.0/src/babble/encoding.py
--rw-r--r--   0        0        0     3969 2023-03-30 10:25:37.450431 fetchai_babble-0.2.0/src/babble/mailbox.py
--rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 fetchai_babble-0.2.0/setup.py
--rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 fetchai_babble-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 15:29:41.621719 fetchai_babble-0.3.0/LICENSE
+-rw-r--r--   0        0        0      730 2023-01-30 14:03:36.544062 fetchai_babble-0.3.0/README.md
+-rw-r--r--   0        0        0      616 2023-07-27 15:08:53.714275 fetchai_babble-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-02-28 15:03:09.430563 fetchai_babble-0.3.0/src/babble/__init__.py
+-rw-r--r--   0        0        0     1594 2023-01-30 14:03:36.548062 fetchai_babble-0.3.0/src/babble/auth.py
+-rw-r--r--   0        0        0     6347 2023-07-27 15:06:25.937247 fetchai_babble-0.3.0/src/babble/client.py
+-rw-r--r--   0        0        0      247 2023-04-27 07:56:38.515274 fetchai_babble-0.3.0/src/babble/config.py
+-rw-r--r--   0        0        0       31 2023-01-30 14:03:36.548062 fetchai_babble-0.3.0/src/babble/crypto/__init__.py
+-rw-r--r--   0        0        0      187 2023-01-30 14:05:08.172852 fetchai_babble-0.3.0/src/babble/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      435 2023-01-30 14:05:08.428854 fetchai_babble-0.3.0/src/babble/crypto/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      528 2023-01-30 14:05:08.428854 fetchai_babble-0.3.0/src/babble/crypto/__pycache__/hashfuncs.cpython-310.pyc
+-rw-r--r--   0        0        0     3373 2023-01-30 14:05:08.176852 fetchai_babble-0.3.0/src/babble/crypto/__pycache__/identity.cpython-310.pyc
+-rw-r--r--   0        0        0       90 2023-01-30 14:03:36.548062 fetchai_babble-0.3.0/src/babble/crypto/exceptions.py
+-rw-r--r--   0        0        0      272 2023-01-30 14:03:36.548062 fetchai_babble-0.3.0/src/babble/crypto/hashfuncs.py
+-rw-r--r--   0        0        0     2911 2023-01-30 14:03:36.548062 fetchai_babble-0.3.0/src/babble/crypto/identity.py
+-rw-r--r--   0        0        0      457 2023-01-30 14:03:36.548062 fetchai_babble-0.3.0/src/babble/encoding.py
+-rw-r--r--   0        0        0     3969 2023-03-30 10:25:37.450431 fetchai_babble-0.3.0/src/babble/mailbox.py
+-rw-r--r--   0        0        0     1664 1970-01-01 00:00:00.000000 fetchai_babble-0.3.0/setup.py
+-rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 fetchai_babble-0.3.0/PKG-INFO
```

### Comparing `fetchai_babble-0.2.0/LICENSE` & `fetchai_babble-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.2.0/README.md` & `fetchai_babble-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.2.0/pyproject.toml` & `fetchai_babble-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fetchai-babble"
-version = "0.2.0"
+version = "0.3.0"
 description = "A simple python library for interacting with the Fetch.ai messaging service (called Memorandum)"
 authors = ["Fetch.AI Limited"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "babble", from = "src" }]
```

### Comparing `fetchai_babble-0.2.0/src/babble/auth.py` & `fetchai_babble-0.3.0/src/babble/auth.py`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.2.0/src/babble/client.py` & `fetchai_babble-0.3.0/src/babble/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from datetime import datetime, timezone
+from datetime import datetime, timezone, timedelta
 from typing import List
 
 import bech32
 
 from .auth import authenticate
 from .crypto.exceptions import RoutingError
 from .crypto.identity import Identity
@@ -11,14 +11,16 @@
 from .mailbox import (
     lookup_messaging_public_key,
     register_messaging_public_key,
     dispatch_messages,
     list_messages,
 )
 
+EXPIRATION_BUFFER_SECONDS = 60 * 5  # 5 minutes
+
 
 def _validate_address(address: str):
     hrp, _ = bech32.bech32_decode(address)
     if hrp is None or hrp not in ("fetch", "agent"):
         raise ValueError(f"Bad delegate address {address}")
 
 
@@ -52,27 +54,38 @@
         self._identity = identity
         self._chain_id = chain_id
 
         # build and restore the delivered set
         self._last_rx_timestamp = self._now()
 
         # authenticate against the API
-        self._token, self._token_metadata = authenticate(self._identity)
+        self._token = None
+        self._update_authentication()
 
         # ensure the registration is in place
         self._update_registration()
 
+    def _update_authentication(self):
+        if (
+            self._token is None
+            or self._token_metadata.expires_at
+            < self._now() - timedelta(seconds=EXPIRATION_BUFFER_SECONDS)
+        ):
+            self._token, self._token_metadata = authenticate(self._identity)
+
     def __repr__(self):
         return f"{self._delegate_address}  ({self._identity.public_key})"
 
     @property
     def delegate_address(self) -> str:
         return self._delegate_address
 
     def send(self, target_address: str, message: str, msg_type: int = 1):
+        self._update_authentication()
+
         target_public_key = lookup_messaging_public_key(
             self._token, target_address, self._chain_id
         )
         if target_public_key is None:
             raise RoutingError(f"Unable to route to {target_address}")
 
         # build up the message structure
@@ -116,14 +129,16 @@
         }
 
         # encode and dispatch the envelope
         enc_envelope = to_base64(to_json(envelope))
         dispatch_messages(self._token, [enc_envelope])
 
     def receive(self) -> List[Message]:
+        self._update_authentication()
+
         output = []
 
         latest_rx_timestamp = self._last_rx_timestamp
 
         # attempt to decode the messages
         for raw_message in list_messages(self._token):
             if raw_message.target != self.delegate_address:
```

### Comparing `fetchai_babble-0.2.0/src/babble/crypto/identity.py` & `fetchai_babble-0.3.0/src/babble/crypto/identity.py`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.2.0/src/babble/mailbox.py` & `fetchai_babble-0.3.0/src/babble/mailbox.py`

 * *Files identical despite different names*

### Comparing `fetchai_babble-0.2.0/setup.py` & `fetchai_babble-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'eciespy>=0.3.13,<0.4.0',
  'pycryptodome>=3.16.0,<4.0.0',
  'pyjwt>=2.6.0,<3.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'fetchai-babble',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A simple python library for interacting with the Fetch.ai messaging service (called Memorandum)',
     'long_description': '# Babble\n\nA simple python library for interacting with the Fetch.ai messaging service (called Memorandum)\n\n## Quick Example\n\n```python\nfrom babble import Client, Identity\n\n# create a set of agents with random identities\nclient1 = Client(\'agent1.....\', Identity.generate())\nclient2 = Client(\'agent1.....\', Identity.generate())\n\n# send a message from one client to another\nclient1.send(client2.delegate_address, "why hello there")\n\n# receive the messages from the other client\nfor msg in client2.receive():\n    print(msg.text)\n```\n\n## Developing\n\n**Install dependencies**\n\n    poetry install\n\n**Run examples**\n\n    poetry run ./examples/simple-e2e.py\n\n**Run tests**\n\n    poetry run pytest\n\n**Run formatter**\n\n    poetry run black .\n',
     'author': 'Fetch.AI Limited',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fetchai_babble-0.2.0/PKG-INFO` & `fetchai_babble-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchai-babble
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple python library for interacting with the Fetch.ai messaging service (called Memorandum)
 License: Apache 2.0
 Author: Fetch.AI Limited
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

