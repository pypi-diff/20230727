# Comparing `tmp/sui_brownie-1.0.9-py3-none-any.whl.zip` & `tmp/sui_brownie-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 28137 bytes, number of entries: 16
+Zip file size: 28190 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12351 b- defN 23-Jun-26 10:12 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    96273 b- defN 23-Jun-26 10:12 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    96650 b- defN 23-Jul-27 05:19 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx     1002 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1297 b- defN 23-Jun-26 10:12 sui_brownie-1.0.9.dist-info/RECORD
-16 files, 162304 bytes uncompressed, 26003 bytes compressed:  84.0%
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-27 05:23 sui_brownie-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 05:23 sui_brownie-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-27 05:23 sui_brownie-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1296 b- defN 23-Jul-27 05:23 sui_brownie-1.1.1.dist-info/RECORD
+16 files, 162660 bytes uncompressed, 26056 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-1.0.9.dist-info/METADATA
+Filename: sui_brownie-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-1.0.9.dist-info/WHEEL
+Filename: sui_brownie-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-1.0.9.dist-info/top_level.txt
+Filename: sui_brownie-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-1.0.9.dist-info/RECORD
+Filename: sui_brownie-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -597,24 +597,35 @@
             cls,
             sender,
             inputs,
             commands,
             gas_price: int,
             gas_budget,
             payment=None,
+            call_args=None
     ) -> IntentMessage:
 
         programmable_transaction = ProgrammableTransaction(inputs, commands)
         if payment is None:
+            if call_args is None:
+                call_args = []
             gases = cls.prepare_gas()
             gas_amount = 0
             payment = []
             for gas in gases:
                 if gas_amount >= gas_budget:
                     break
+                is_filter = False
+                for call_arg in call_args:
+                    if gas["coinObjectId"] == call_arg:
+                        is_filter = True
+                        break
+                if is_filter:
+                    continue
+
                 payment.append(ObjectRef(
                     ObjectID(gas["coinObjectId"]),
                     SequenceNumber(int(gas["version"])),
                     ObjectDigest(gas["digest"])
                 ))
                 gas_amount += int(gas["balance"])
 
@@ -650,15 +661,15 @@
             abi,
             type_args,
             call_args,
             gas_price: int,
             gas_budget,
     ) -> IntentMessage:
         inputs, commands = cls.command_move_call(package_id, abi, type_args, call_args)
-        return cls.build_intent_message(sender, inputs, commands, gas_price, gas_budget)
+        return cls.build_intent_message(sender, inputs, commands, gas_price, gas_budget, call_args=call_args)
 
     @classmethod
     def transfer_object(
             cls,
             sender,
             object_id,
             recipient,
```

## Comparing `sui_brownie-1.0.9.dist-info/METADATA` & `sui_brownie-1.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 1.0.9
+Version: 1.1.1
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -24,9 +23,7 @@
 Requires-Dist: retrying
 Requires-Dist: mnemonic
 Requires-Dist: httpx
 Requires-Dist: python-dotenv
 Requires-Dist: pynacl
 
 This is an sui python tool to quickly implement sui calls
-
-
```

## Comparing `sui_brownie-1.0.9.dist-info/RECORD` & `sui_brownie-1.1.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=KZ-hx82tKH6MyMYXZqeh1JOSbrEBRHqDgWGOLJQxiXc,12351
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=xSpnsFpR6Hll6-UBRpHn2-LVwLN7YusX2D2GcoXeTYI,96273
+sui_brownie/sui_brownie.py,sha256=77k5qykCTiLGH8B3-8UUQzhZVYAqV92BDRsHIExe9v8,96650
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-1.0.9.dist-info/METADATA,sha256=IvCQQyv1WZKkq-5KAIps2w9S-9r1uMQbJWwGtPo1UlE,1002
-sui_brownie-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-1.0.9.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-1.0.9.dist-info/RECORD,,
+sui_brownie-1.1.1.dist-info/METADATA,sha256=MjW-stfb_pO5gXnELF7PMJ9o1SrmBguEwIU47MFjzzc,982
+sui_brownie-1.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-1.1.1.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-1.1.1.dist-info/RECORD,,
```

