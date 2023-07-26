# Comparing `tmp/alice_blue-2.0.3-py2.py3-none-any.whl.zip` & `tmp/alice_blue-2.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 35039 bytes, number of entries: 7
--rw-r--r--  2.0 unx      247 b- defN 22-Oct-08 15:55 alice_blue/__init__.py
--rw-r--r--  2.0 unx    53847 b- defN 22-Oct-08 15:55 alice_blue/alice_blue.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Oct-08 15:57 alice_blue-2.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    43773 b- defN 22-Oct-08 15:57 alice_blue-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Oct-08 15:57 alice_blue-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Oct-08 15:57 alice_blue-2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 22-Oct-08 15:57 alice_blue-2.0.3.dist-info/RECORD
-7 files, 133705 bytes uncompressed, 34037 bytes compressed:  74.5%
+Zip file size: 35054 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      275 b- defN 23-Jul-26 23:33 alice_blue/__init__.py
+-rw-r--r--  2.0 unx    53848 b- defN 23-Jul-26 23:33 alice_blue/alice_blue.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-26 23:35 alice_blue-2.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    43773 b- defN 23-Jul-26 23:35 alice_blue-2.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-26 23:35 alice_blue-2.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-26 23:35 alice_blue-2.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      568 b- defN 23-Jul-26 23:35 alice_blue-2.0.4.dist-info/RECORD
+7 files, 133734 bytes uncompressed, 34052 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: alice_blue/__init__.py
 Comment: 
 
 Filename: alice_blue/alice_blue.py
 Comment: 
 
-Filename: alice_blue-2.0.3.dist-info/LICENSE.txt
+Filename: alice_blue-2.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: alice_blue-2.0.3.dist-info/METADATA
+Filename: alice_blue-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: alice_blue-2.0.3.dist-info/WHEEL
+Filename: alice_blue-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: alice_blue-2.0.3.dist-info/top_level.txt
+Filename: alice_blue-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: alice_blue-2.0.3.dist-info/RECORD
+Filename: alice_blue-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alice_blue/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .alice_blue import AliceBlue, TransactionType, OrderType, ProductType, LiveFeedType, Instrument, HistoricalDataType
-__all__ = ['AliceBlue', 'TransactionType', 'OrderType', 'ProductType', 'LiveFeedType', 'Instrument', 'HistoricalDataType'] 
+from .alice_blue import AliceBlue, TransactionType, OrderType, ProductType, LiveFeedType, Instrument, HistoricalDataType, CryptoJsAES
+__all__ = ['AliceBlue', 'TransactionType', 'OrderType', 'ProductType', 'LiveFeedType', 'Instrument', 'HistoricalDataType', 'CryptoJsAES']
```

## alice_blue/alice_blue.py

```diff
@@ -91,15 +91,15 @@
         aes = Cipher(algorithms.AES(key), modes.CBC(iv))
         return CryptoJsAES.__unpad(aes.decryptor.update(encrypted[16:]) + aes.decryptor().finalize())
 
 class AliceBlue:
     """ AliceBlue Class for all operations related to AliceBlue Server"""
 
     # URLs
-    host = "https://a3.aliceblueonline.com/rest/AliceBlueAPIService"
+    host = "https://ant.aliceblueonline.com/rest/AliceBlueAPIService"
     __urls = {  "webLogin"              :   f"{host}/customer/webLogin",
                 "twoFA"                 :   f"{host}/sso/validAnswer",
                 "sessionID"             :   f"{host}/sso/getUserDetails",
                 "getEncKey"             :   f"{host}/customer/getEncryptionKey",
                 "authorizeVendor"       :   f"{host}/sso/authorizeVendor",
                 "apiGetEncKey"          :   f"{host}/api/customer/getAPIEncpkey",
                 "profile"               :   f"{host}/api/customer/accountDetails",
```

## Comparing `alice_blue-2.0.3.dist-info/LICENSE.txt` & `alice_blue-2.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `alice_blue-2.0.3.dist-info/METADATA` & `alice_blue-2.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alice-blue
-Version: 2.0.3
+Version: 2.0.4
 Summary: Official Python library for Alice Blue APIs
 Home-page: https://github.com/krishnavelu/alice_blue
 Author: Krishna Velu
 Author-email: krishnajvelu@gmail.com
 License: UNKNOWN
 Keywords: alice,alice-blue,python,sdk,trading,stock markets
 Platform: UNKNOWN
```

## Comparing `alice_blue-2.0.3.dist-info/RECORD` & `alice_blue-2.0.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-alice_blue/__init__.py,sha256=ZF5m6fNI-ec-YnasIgbXSemSHsPYR8ORImPpJ_egkgg,247
-alice_blue/alice_blue.py,sha256=oSZXa9M3pCCImMol6HU5T9gvUHU4glSKoYaChcpcJfY,53847
-alice_blue-2.0.3.dist-info/LICENSE.txt,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-alice_blue-2.0.3.dist-info/METADATA,sha256=-XuDKThNzCetXvacDXOZ6lT1w9mkWItvBO7Ib_WTsbc,43773
-alice_blue-2.0.3.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-alice_blue-2.0.3.dist-info/top_level.txt,sha256=kfn7JBQMuws2dg9F8ch4LZIGhVtB5rJ9CmXiodGXHh0,11
-alice_blue-2.0.3.dist-info/RECORD,,
+alice_blue/__init__.py,sha256=ykZcHkuCbRoBlpR2Atln7FJVjNb2L4kORxUUP8bXD9s,275
+alice_blue/alice_blue.py,sha256=hNyYBfoA9t8_DCqrEMAhFvlkBFR5UBZft1nwNWRuEhQ,53848
+alice_blue-2.0.4.dist-info/LICENSE.txt,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+alice_blue-2.0.4.dist-info/METADATA,sha256=0HGWT6LVsOho0D60-vFOiFCr40jcwUCbcZMuyx8HySo,43773
+alice_blue-2.0.4.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+alice_blue-2.0.4.dist-info/top_level.txt,sha256=kfn7JBQMuws2dg9F8ch4LZIGhVtB5rJ9CmXiodGXHh0,11
+alice_blue-2.0.4.dist-info/RECORD,,
```

