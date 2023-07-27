# Comparing `tmp/metathing-0.3.4-py3-none-any.whl.zip` & `tmp/metathing-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23088 bytes, number of entries: 14
+Zip file size: 23109 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-16 20:12 metathing/__init__.py
 -rw-r--r--  2.0 unx     2210 b- defN 23-Jul-16 20:12 metathing/alarmer.py
--rw-r--r--  2.0 unx    10859 b- defN 23-Jul-23 22:29 metathing/application.py
+-rw-r--r--  2.0 unx    10855 b- defN 23-Jul-27 18:14 metathing/application.py
 -rw-r--r--  2.0 unx      290 b- defN 23-Jul-16 20:12 metathing/config.py
 -rw-r--r--  2.0 unx    20160 b- defN 23-Jul-18 05:14 metathing/device.py
 -rw-r--r--  2.0 unx    16120 b- defN 23-Jul-17 07:21 metathing/http.py
 -rw-r--r--  2.0 unx     1520 b- defN 23-Jul-17 09:21 metathing/logger.py
--rw-r--r--  2.0 unx    21631 b- defN 23-Jul-20 01:11 metathing/metathing.py
+-rw-r--r--  2.0 unx    21636 b- defN 23-Jul-27 18:25 metathing/metathing.py
 -rw-r--r--  2.0 unx     6946 b- defN 23-Jul-17 07:21 metathing/mqtt.py
 -rw-r--r--  2.0 unx     3990 b- defN 23-Jul-17 07:22 metathing/service.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/RECORD
-14 files, 85064 bytes uncompressed, 21334 bytes compressed:  74.9%
+-rw-r--r--  2.0 unx      163 b- defN 23-Jul-27 18:26 metathing-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 18:26 metathing-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-27 18:26 metathing-0.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-27 18:26 metathing-0.3.6.dist-info/RECORD
+14 files, 85065 bytes uncompressed, 21355 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: metathing/mqtt.py
 Comment: 
 
 Filename: metathing/service.py
 Comment: 
 
-Filename: metathing-0.3.4.dist-info/METADATA
+Filename: metathing-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: metathing-0.3.4.dist-info/WHEEL
+Filename: metathing-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: metathing-0.3.4.dist-info/top_level.txt
+Filename: metathing-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: metathing-0.3.4.dist-info/RECORD
+Filename: metathing-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metathing/application.py

```diff
@@ -151,15 +151,15 @@
             else:
                 return False
         return item
     
     def _processing_model(self, res: str):
         try:
             if res == 'null' or res is None:
-                self._print_frame(["* Service has not been registered in MTNode *"])
+                self._print_frame(["@* 无法获取服务的适配模型！ *"])
                 return None
             model = json.loads(res)
             self.model = model
             message = [
                 f"-= {self.srv.srv_name} =-",
                 f"UID: {model['uid']}",
             ]
```

## metathing/metathing.py

```diff
@@ -103,15 +103,15 @@
         def gen_adapter_var(item):
             return {
                 "srv_id": self.srv.srv_name,
                 "var_tag": item['var_name'],
                 "name": item['name'],
                 "name@zh": item['name@zh'] if 'name@zh' in item else item['name'],
                 "dtype": item['dtype'],
-                "default": item['default'] if 'default' in item else None,
+                "default": str(item['default']) if 'default' in item else None,
                 "dgraph.type": "AdapterVar",
             }
             
         def gen_adapter_fn(fn_name, item, is_act, is_global):
             res = {
                 "srv_id": self.srv.srv_name,
                 "name": item['name'],
```

## Comparing `metathing-0.3.4.dist-info/RECORD` & `metathing-0.3.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 metathing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 metathing/alarmer.py,sha256=qXCTl8zw3UTqbDqvvPAHU-a1uJqxlAkxzQWf-5nVB3Q,2210
-metathing/application.py,sha256=K5juHHwfQ9n9hGkRZ3NJZvazYLVb_w3msT79S7bxEp0,10859
+metathing/application.py,sha256=E-v5lWNsfYDZpVIDIcyQbkGERHGW8iVHEb22Ddf7zTs,10855
 metathing/config.py,sha256=SZs7VXZeNQ4BwexSjsB_YJk6CPNwNMyvEpaXlztea-s,290
 metathing/device.py,sha256=8HzJv7zCm1FthWrwvPKK823rhY4J3Q7iKtin79lNK5c,20160
 metathing/http.py,sha256=xaTP2BHFxd9BTMHoM_grY_O9kzhip608P0RfivmDo0A,16120
 metathing/logger.py,sha256=ZX1t9Yuibg6Ortkimet3h2DxrnQCpSszvrFrJZQYXPc,1520
-metathing/metathing.py,sha256=eYXA_XNFlTtXonphPH25fo0IStaBuvjtyBntSggRM-k,21631
+metathing/metathing.py,sha256=EYsMWXRcDk7KkDYMcl6zN0ymC6dCNg4w-tUoOsZPKNk,21636
 metathing/mqtt.py,sha256=05DvcdV46YeWiBFpI3LWL2frQCrvJXqf8_VYPC-iyyY,6946
 metathing/service.py,sha256=OOTjDLb00s1mRSLg2q4egbZDAUevz_IueL63el-I8u4,3990
-metathing-0.3.4.dist-info/METADATA,sha256=D8470azsuXbUkEXdad3lYzUockulrki__ua2b6p6MJQ,163
-metathing-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-metathing-0.3.4.dist-info/top_level.txt,sha256=O2krbfropyUTFNX_RrOEn4VwPiaKXYRwSNjbuj31gP8,10
-metathing-0.3.4.dist-info/RECORD,,
+metathing-0.3.6.dist-info/METADATA,sha256=rr0tEGFxio38HoupRamR4_l-1BjaPmTxbBS32e0kQn0,163
+metathing-0.3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+metathing-0.3.6.dist-info/top_level.txt,sha256=O2krbfropyUTFNX_RrOEn4VwPiaKXYRwSNjbuj31gP8,10
+metathing-0.3.6.dist-info/RECORD,,
```

