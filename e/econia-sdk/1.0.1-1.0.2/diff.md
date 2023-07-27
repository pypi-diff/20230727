# Comparing `tmp/econia_sdk-1.0.1.tar.gz` & `tmp/econia_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econia_sdk-1.0.1.tar", max compression
+gzip compressed data, was "econia_sdk-1.0.2.tar", max compression
```

## Comparing `econia_sdk-1.0.1.tar` & `econia_sdk-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       61 2023-07-27 15:12:20.104373 econia_sdk-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854900 econia_sdk-1.0.1/econia_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854950 econia_sdk-1.0.1/econia_sdk/entry/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-21 16:14:17.855021 econia_sdk-1.0.1/econia_sdk/entry/incentives.py
--rw-r--r--   0        0        0     9304 2023-07-26 14:37:08.196179 econia_sdk-1.0.1/econia_sdk/entry/market.py
--rw-r--r--   0        0        0     3637 2023-07-21 16:14:17.855149 econia_sdk-1.0.1/econia_sdk/entry/registry.py
--rw-r--r--   0        0        0     3883 2023-07-21 16:14:17.855205 econia_sdk-1.0.1/econia_sdk/entry/user.py
--rw-r--r--   0        0        0     3534 2023-07-26 14:37:08.196402 econia_sdk-1.0.1/econia_sdk/lib.py
--rw-r--r--   0        0        0      551 2023-07-27 00:22:09.389353 econia_sdk-1.0.1/econia_sdk/types.py
--rw-r--r--   0        0        0        0 2023-07-26 14:37:08.196805 econia_sdk-1.0.1/econia_sdk/view/__init__.py
--rw-r--r--   0        0        0     2639 2023-07-26 14:37:08.196949 econia_sdk-1.0.1/econia_sdk/view/incentives.py
--rw-r--r--   0        0        0     6789 2023-07-26 14:37:08.197100 econia_sdk-1.0.1/econia_sdk/view/market.py
--rw-r--r--   0        0        0     6936 2023-07-26 14:37:08.197229 econia_sdk-1.0.1/econia_sdk/view/registry.py
--rw-r--r--   0        0        0      263 2023-07-26 14:37:08.197565 econia_sdk-1.0.1/econia_sdk/view/resource_account.py
--rw-r--r--   0        0        0    17155 2023-07-27 15:12:20.104864 econia_sdk-1.0.1/econia_sdk/view/user.py
--rw-r--r--   0        0        0      388 2023-07-27 15:14:12.022137 econia_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 econia_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-27 18:10:49.224251 econia_sdk-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854900 econia_sdk-1.0.2/econia_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:14:17.854950 econia_sdk-1.0.2/econia_sdk/entry/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-21 16:14:17.855021 econia_sdk-1.0.2/econia_sdk/entry/incentives.py
+-rw-r--r--   0        0        0     9305 2023-07-27 18:56:10.502928 econia_sdk-1.0.2/econia_sdk/entry/market.py
+-rw-r--r--   0        0        0     3637 2023-07-21 16:14:17.855149 econia_sdk-1.0.2/econia_sdk/entry/registry.py
+-rw-r--r--   0        0        0     3883 2023-07-21 16:14:17.855205 econia_sdk-1.0.2/econia_sdk/entry/user.py
+-rw-r--r--   0        0        0     3534 2023-07-26 14:37:08.196402 econia_sdk-1.0.2/econia_sdk/lib.py
+-rw-r--r--   0        0        0      551 2023-07-27 00:22:09.389353 econia_sdk-1.0.2/econia_sdk/types.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:37:08.196805 econia_sdk-1.0.2/econia_sdk/view/__init__.py
+-rw-r--r--   0        0        0     2640 2023-07-27 18:56:10.506615 econia_sdk-1.0.2/econia_sdk/view/incentives.py
+-rw-r--r--   0        0        0     6790 2023-07-27 18:56:10.513134 econia_sdk-1.0.2/econia_sdk/view/market.py
+-rw-r--r--   0        0        0     8509 2023-07-27 18:56:26.619749 econia_sdk-1.0.2/econia_sdk/view/registry.py
+-rw-r--r--   0        0        0      264 2023-07-27 18:56:10.514681 econia_sdk-1.0.2/econia_sdk/view/resource_account.py
+-rw-r--r--   0        0        0    17151 2023-07-27 18:56:10.509675 econia_sdk-1.0.2/econia_sdk/view/user.py
+-rw-r--r--   0        0        0      409 2023-07-27 19:04:47.825946 econia_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 econia_sdk-1.0.2/PKG-INFO
```

### Comparing `econia_sdk-1.0.1/econia_sdk/entry/incentives.py` & `econia_sdk-1.0.2/econia_sdk/entry/incentives.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.1/econia_sdk/entry/market.py` & `econia_sdk-1.0.2/econia_sdk/entry/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Market entry functions
 
 from aptos_sdk.account_address import AccountAddress
 from aptos_sdk.bcs import Serializer, encoder
 from aptos_sdk.transactions import EntryFunction, ModuleId
 from aptos_sdk.type_tag import TypeTag
+
 from econia_sdk.types import AdvanceStyle, Restriction, SelfMatchBehavior, Side
 
 
 def get_module_id(econia_address: AccountAddress) -> ModuleId:
     return ModuleId.from_str("{}::market".format(econia_address))
```

### Comparing `econia_sdk-1.0.1/econia_sdk/entry/registry.py` & `econia_sdk-1.0.2/econia_sdk/entry/registry.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.1/econia_sdk/entry/user.py` & `econia_sdk-1.0.2/econia_sdk/entry/user.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.1/econia_sdk/lib.py` & `econia_sdk-1.0.2/econia_sdk/lib.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.1/econia_sdk/types.py` & `econia_sdk-1.0.2/econia_sdk/types.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-1.0.1/econia_sdk/view/incentives.py` & `econia_sdk-1.0.2/econia_sdk/view/incentives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from aptos_sdk.account_address import AccountAddress
+
 from econia_sdk.lib import EconiaViewer
 
 
 def get_cost_to_upgrade_integrator_fee_store_view(
     view: EconiaViewer,
     quote_coin_type: str,
     utility_coin_type: str,
```

### Comparing `econia_sdk-1.0.1/econia_sdk/view/market.py` & `econia_sdk-1.0.2/econia_sdk/view/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Optional
 
 from aptos_sdk.account_address import AccountAddress
+
 from econia_sdk.lib import EconiaViewer
 from econia_sdk.types import Side
 
 _HI_64 = 18446744073709551615
 
 
 def get_ABORT(view: EconiaViewer) -> int:
```

### Comparing `econia_sdk-1.0.1/econia_sdk/view/registry.py` & `econia_sdk-1.0.2/econia_sdk/view/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Optional
 
 from aptos_sdk.account_address import AccountAddress
+
 from econia_sdk.lib import EconiaViewer
 
 
 def get_MAX_CHARACTERS_GENERIC(view: EconiaViewer) -> int:
     returns = view.get_returns(
         "registry",
         "get_MAX_CHARACTERS_GENERIC",
@@ -44,42 +45,82 @@
     value = returns[0]
     return {
         "n_markets": int(value["n_markets"]),
         "n_recognized_markets": int(value["n_recognized_markets"]),
     }
 
 
-def get_market_info(view: EconiaViewer, market_id: int) -> dict:
+class GetMarketInfoReturn(dict):
+    def is_coin_market(self, viewer: EconiaViewer) -> bool:
+        base_info = self["base_type"]
+        is_econia = viewer.econia_address.hex() == base_info["package_address"]
+        is_generic = (
+            base_info["module_name"] == "registry"
+            and base_info["type_name"] == "GenericAsset"
+        )
+        return not (is_econia and is_generic)
+
+    def get_decimals_base(self, viewer: EconiaViewer):
+        assert self.is_coin_market(
+            viewer
+        ), "Generic market has no decimals for base type!"
+        return self._get_decimals(viewer, self["base_type"])
+
+    def get_decimals_quote(self, viewer: EconiaViewer):
+        return self._get_decimals(viewer, self["quote_type"])
+
+    def _get_decimals(self, viewer: EconiaViewer, type_info: dict):
+        request = f"{viewer.aptos_client.base_url}/view"
+        address = type_info["package_address"].hex()
+        module = type_info["module_name"]
+        type_name = type_info["type_name"]
+        response = viewer.aptos_client.client.post(
+            request,
+            json={
+                "function": f"0x1::coin::decimals",
+                "type_arguments": [f"{address}::{module}::{type_name}"],
+                "arguments": [],
+            },
+        )
+
+        if response.status_code >= 400:
+            raise Exception(response.text, response.status_code)
+        return int(response.json()[0])
+
+
+def get_market_info(view: EconiaViewer, market_id: int) -> GetMarketInfoReturn:
     returns = view.get_returns(
         "registry", "get_market_info", [], [str(market_id)]
     )
     value = returns[0]
-    return {
-        "base_name_generic": value["base_name_generic"],
-        "base_type": {
-            "module_name": value["base_type"]["module_name"],
-            "package_address": AccountAddress.from_hex(
-                value["base_type"]["package_address"]
-            ),
-            "type_name": value["base_type"]["type_name"],
-        },
-        "is_recognized": bool(value["is_recognized"]),
-        "lot_size": int(value["lot_size"]),  # subunits of base
-        "market_id": int(value["market_id"]),
-        "min_size": int(value["min_size"]),
-        "quote_type": {
-            "module_name": value["quote_type"]["module_name"],
-            "package_address": AccountAddress.from_hex(
-                value["quote_type"]["package_address"]
-            ),
-            "type_name": value["quote_type"]["type_name"],
-        },
-        "tick_size": int(value["tick_size"]),
-        "underwriter_id": int(value["underwriter_id"]),
-    }
+    return GetMarketInfoReturn(
+        {
+            "base_name_generic": value["base_name_generic"],
+            "base_type": {
+                "module_name": value["base_type"]["module_name"],
+                "package_address": AccountAddress.from_hex(
+                    value["base_type"]["package_address"]
+                ),
+                "type_name": value["base_type"]["type_name"],
+            },
+            "is_recognized": bool(value["is_recognized"]),
+            "lot_size": int(value["lot_size"]),  # subunits of base
+            "market_id": int(value["market_id"]),
+            "min_size": int(value["min_size"]),
+            "quote_type": {
+                "module_name": value["quote_type"]["module_name"],
+                "package_address": AccountAddress.from_hex(
+                    value["quote_type"]["package_address"]
+                ),
+                "type_name": value["quote_type"]["type_name"],
+            },
+            "tick_size": int(value["tick_size"]),
+            "underwriter_id": int(value["underwriter_id"]),
+        }
+    )
 
 
 def get_recognized_market_id_base_coin(
     view: EconiaViewer,
     base_coin_type: str,
     quote_coin_type: str,
 ) -> int:
```

### Comparing `econia_sdk-1.0.1/econia_sdk/view/user.py` & `econia_sdk-1.0.2/econia_sdk/view/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Any, List, Optional
+from typing import List, Optional
 
 from aptos_sdk.account_address import AccountAddress
+
 from econia_sdk.lib import EconiaViewer
 from econia_sdk.types import CancelReason, Restriction, SelfMatchBehavior, Side
 
 
 def get_ASK(view: EconiaViewer) -> bool:
     returns = view.get_returns("user", "get_ASK")
     return bool(returns[0])
```

