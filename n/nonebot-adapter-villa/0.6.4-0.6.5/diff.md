# Comparing `tmp/nonebot_adapter_villa-0.6.4.tar.gz` & `tmp/nonebot_adapter_villa-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.6.4.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.6.5.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.6.4.tar` & `nonebot_adapter_villa-0.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/LICENSE
--rw-r--r--   0        0        0     7323 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/README.md
--rw-r--r--   0        0        0      228 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    12302 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0       25 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0     3293 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/client.pyi
--rw-r--r--   0        0        0    13152 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9568 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1734 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    14504 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0     1190 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    12798 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     2717 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     9952 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0     1449 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/permission.py
--rw-r--r--   0        0        0       76 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     2125 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-27 10:18:08.947032 nonebot_adapter_villa-0.6.5/LICENSE
+-rw-r--r--   0        0        0     7323 2023-07-27 10:18:08.947032 nonebot_adapter_villa-0.6.5/README.md
+-rw-r--r--   0        0        0      228 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    12302 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0     3316 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/client.pyi
+-rw-r--r--   0        0        0    13179 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9568 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1734 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    14504 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0     1190 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    12798 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     2717 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     9952 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1449 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-27 10:18:08.951032 nonebot_adapter_villa-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.5/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.6.4/LICENSE` & `nonebot_adapter_villa-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/README.md` & `nonebot_adapter_villa-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/client.pyi` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -115,9 +115,10 @@
         pass_through: str,
         room_id: int,
         uid: int,
     ) -> str: ...
     async def transfer_image(
         self,
         *,
+        villa_id: int,
         url: str,
     ) -> str: ...
```

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,20 +431,21 @@
     )
     return (await _request(adapter, bot, request))["audit_id"]
 
 
 async def _transfer_image(
     adapter: "Adapter",
     bot: "Bot",
+    villa_id: int,
     url: str,
 ) -> str:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/transferImage",
-        headers=bot.get_authorization_header(),
+        headers=bot.get_authorization_header(villa_id),
         json={
             "url": url,
         },
     )
     return (await _request(adapter, bot, request))["new_url"]
```

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/permission.py` & `nonebot_adapter_villa-0.6.5/nonebot/adapters/villa/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.4/pyproject.toml` & `nonebot_adapter_villa-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.6.4"
+version = "0.6.5"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.6.4/PKG-INFO` & `nonebot_adapter_villa-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.6.4
+Version: 0.6.5
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.5 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

