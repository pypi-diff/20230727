# Comparing `tmp/nonebot_adapter_villa-0.6.3.tar.gz` & `tmp/nonebot_adapter_villa-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.6.3.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.6.4.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.6.3.tar` & `nonebot_adapter_villa-0.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/LICENSE
--rw-r--r--   0        0        0     7323 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/README.md
--rw-r--r--   0        0        0      228 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    12302 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0       25 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0     3293 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/client.pyi
--rw-r--r--   0        0        0    13152 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9534 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1734 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    14504 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0     1190 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    12798 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     2717 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     9952 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0     1449 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/permission.py
--rw-r--r--   0        0        0       76 2023-07-23 07:05:16.999946 nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     2125 2023-07-23 07:05:17.003946 nonebot_adapter_villa-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/LICENSE
+-rw-r--r--   0        0        0     7323 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/README.md
+-rw-r--r--   0        0        0      228 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    12302 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0     3293 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/client.pyi
+-rw-r--r--   0        0        0    13152 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9568 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1734 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    14504 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0     1190 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    12798 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     2717 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     9952 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1449 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-27 08:05:17.666576 nonebot_adapter_villa-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.4/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.6.3/LICENSE` & `nonebot_adapter_villa-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/README.md` & `nonebot_adapter_villa-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/client.pyi` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     bot_secret: str
 
 
 # http事件回调部分
 # see https://webstatic.mihoyo.com/vila/bot/doc/callback.html
 class Command(BaseModel):
     name: str
-    desc: str
+    desc: Optional[str] = None
 
 
 class Template(BaseModel):
     id: str
     name: str
-    desc: str
+    desc: Optional[str] = None
     icon: str
     commands: Optional[List[Command]] = None
 
 
 class Robot(BaseModel):
     villa_id: int
     template: Template
```

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/nonebot/adapters/villa/permission.py` & `nonebot_adapter_villa-0.6.4/nonebot/adapters/villa/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.3/pyproject.toml` & `nonebot_adapter_villa-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.6.3"
+version = "0.6.4"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.6.3/PKG-INFO` & `nonebot_adapter_villa-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.6.3
+Version: 0.6.4
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
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.4 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

