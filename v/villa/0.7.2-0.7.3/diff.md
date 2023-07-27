# Comparing `tmp/villa-0.7.2.tar.gz` & `tmp/villa-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.7.2.tar", max compression
+gzip compressed data, was "villa-0.7.3.tar", max compression
```

## Comparing `villa-0.7.2.tar` & `villa-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-07-21 07:44:11.656905 villa-0.7.2/LICENSE
--rw-r--r--   0        0        0     3747 2023-07-21 07:44:11.656905 villa-0.7.2/README.md
--rw-r--r--   0        0        0     2140 2023-07-21 07:44:11.656905 villa-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      277 2023-07-21 07:44:11.656905 villa-0.7.2/villa/__init__.py
--rw-r--r--   0        0        0    40762 2023-07-21 07:44:11.656905 villa-0.7.2/villa/bot.py
--rw-r--r--   0        0        0    12215 2023-07-21 07:44:11.656905 villa-0.7.2/villa/event.py
--rw-r--r--   0        0        0     1835 2023-07-21 07:44:11.656905 villa-0.7.2/villa/exception.py
--rw-r--r--   0        0        0     3337 2023-07-21 07:44:11.656905 villa-0.7.2/villa/handle.py
--rw-r--r--   0        0        0     1537 2023-07-21 07:44:11.656905 villa-0.7.2/villa/log.py
--rw-r--r--   0        0        0    21359 2023-07-21 07:44:11.656905 villa-0.7.2/villa/message.py
--rw-r--r--   0        0        0     9350 2023-07-21 07:44:11.656905 villa-0.7.2/villa/models.py
--rw-r--r--   0        0        0      935 2023-07-21 07:44:11.656905 villa-0.7.2/villa/store.py
--rw-r--r--   0        0        0      240 2023-07-21 07:44:11.656905 villa-0.7.2/villa/typing.py
--rw-r--r--   0        0        0     1534 2023-07-21 07:44:11.656905 villa-0.7.2/villa/utils.py
--rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 villa-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-27 08:16:29.105593 villa-0.7.3/LICENSE
+-rw-r--r--   0        0        0     3747 2023-07-27 08:16:29.105593 villa-0.7.3/README.md
+-rw-r--r--   0        0        0     2140 2023-07-27 08:16:29.109593 villa-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-07-27 08:16:29.109593 villa-0.7.3/villa/__init__.py
+-rw-r--r--   0        0        0    40762 2023-07-27 08:16:29.109593 villa-0.7.3/villa/bot.py
+-rw-r--r--   0        0        0    12215 2023-07-27 08:16:29.109593 villa-0.7.3/villa/event.py
+-rw-r--r--   0        0        0     1835 2023-07-27 08:16:29.109593 villa-0.7.3/villa/exception.py
+-rw-r--r--   0        0        0     3337 2023-07-27 08:16:29.109593 villa-0.7.3/villa/handle.py
+-rw-r--r--   0        0        0     1537 2023-07-27 08:16:29.109593 villa-0.7.3/villa/log.py
+-rw-r--r--   0        0        0    21359 2023-07-27 08:16:29.109593 villa-0.7.3/villa/message.py
+-rw-r--r--   0        0        0     9384 2023-07-27 08:16:29.109593 villa-0.7.3/villa/models.py
+-rw-r--r--   0        0        0      935 2023-07-27 08:16:29.109593 villa-0.7.3/villa/store.py
+-rw-r--r--   0        0        0      240 2023-07-27 08:16:29.109593 villa-0.7.3/villa/typing.py
+-rw-r--r--   0        0        0     1534 2023-07-27 08:16:29.109593 villa-0.7.3/villa/utils.py
+-rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 villa-0.7.3/PKG-INFO
```

### Comparing `villa-0.7.2/LICENSE` & `villa-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/README.md` & `villa-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/pyproject.toml` & `villa-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.7.2"
+version = "0.7.3"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.7.2/villa/bot.py` & `villa-0.7.3/villa/bot.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/villa/event.py` & `villa-0.7.3/villa/event.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/villa/exception.py` & `villa-0.7.3/villa/exception.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/villa/handle.py` & `villa-0.7.3/villa/handle.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/villa/log.py` & `villa-0.7.3/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/villa/message.py` & `villa-0.7.3/villa/message.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/villa/models.py` & `villa-0.7.3/villa/models.py`

 * *Files 2% similar despite different names*

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

### Comparing `villa-0.7.2/villa/store.py` & `villa-0.7.3/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/villa/utils.py` & `villa-0.7.3/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.7.2/PKG-INFO` & `villa-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.7.2
+Version: 0.7.3
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

