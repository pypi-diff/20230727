# Comparing `tmp/lite_fastapi_local-0.0.41.tar.gz` & `tmp/lite_fastapi_local-0.0.42.tar.gz`

## Comparing `lite_fastapi_local-0.0.41.tar` & `lite_fastapi_local-0.0.42.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/QR_READ_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/__init__.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/requirements.txt
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/common/__init__.py
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/common/function.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/common/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/boxDoorModel.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/drimmLedModel.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/innerLedModel.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/motorModel.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/registrationModel.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/setupModel.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/solModel.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/sprayModel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/router/__init__.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/router/motorRouter.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/router/sensorRouter.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/src/lite_fastapi_local/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.41/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/__init__.py
+-rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/common/__init__.py
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/drimmLedModel.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/innerLedModel.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/registrationModel.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/router/__init__.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.42/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/QR_CHK_dep.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/QR_READ_dep.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/main.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,20 +90,20 @@
     
 @mqtt.subscribe("tg/#")
 async def message_to_topic(client, topic, payload, qos, properties):
     if common.get_MACHINE_MAC():
         return
     mac_address = topic.split('/')[1]
     common.set_MACHINE_MAC(mac_address)
-    registration.register_iot_core_by_mac_address()
     # common.set_MACHINE_MAC(data["MAC"])
     # data = json.loads(payload.decode())
     mqtt.client.unsubscribe("tg/#")
     mqtt.client.subscribe(f"tg/{mac_address}/#")
-    print('get mac address!!')
+    registration.register_iot_core_by_mac_address()
+    print(f'get mac address : {mac_address}')
     
 @app.get('/', response_class=PlainTextResponse)
 def read_root():
     common.clear_returned_qr_code_list()
     return 'THE GREET'
 
 @app.get('/QR_READ', response_class=PlainTextResponse)
```

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/requirements.txt` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/settings.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/common/function.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/common/function.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/common/variable.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/motorModel.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/setupModel.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/setupModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/model/solModel.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/router/motorRouter.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/router/motorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/router/sensorRouter.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/src/lite_fastapi_local/router/setupRouter.py` & `lite_fastapi_local-0.0.42/src/lite_fastapi_local/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/LICENSE` & `lite_fastapi_local-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.41/pyproject.toml` & `lite_fastapi_local-0.0.42/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.41"
+version = "0.0.42"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.41/PKG-INFO` & `lite_fastapi_local-0.0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.41
+Version: 0.0.42
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

