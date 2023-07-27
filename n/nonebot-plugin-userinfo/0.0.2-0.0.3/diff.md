# Comparing `tmp/nonebot_plugin_userinfo-0.0.2.tar.gz` & `tmp/nonebot_plugin_userinfo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_userinfo-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_userinfo-0.0.3.tar", max compression
```

## Comparing `nonebot_plugin_userinfo-0.0.2.tar` & `nonebot_plugin_userinfo-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/LICENSE
--rw-r--r--   0        0        0     2680 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/README.md
--rw-r--r--   0        0        0      699 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/__init__.py
--rw-r--r--   0        0        0       75 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/__init__.py
--rw-r--r--   0        0        0     1008 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/console.py
--rw-r--r--   0        0        0     1850 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/kaiheila.py
--rw-r--r--   0        0        0     1723 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3940 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v12.py
--rw-r--r--   0        0        0     1968 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/qqguild.py
--rw-r--r--   0        0        0     3472 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/telegram.py
--rw-r--r--   0        0        0       40 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/exception.py
--rw-r--r--   0        0        0     2447 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/getter.py
--rw-r--r--   0        0        0     2066 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/image_source.py
--rw-r--r--   0        0        0      324 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/user_info.py
--rw-r--r--   0        0        0      565 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/utils.py
--rw-r--r--   0        0        0     1620 2023-06-30 03:35:48.781446 nonebot_plugin_userinfo-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 nonebot_plugin_userinfo-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2680 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/README.md
+-rw-r--r--   0        0        0      699 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/__init__.py
+-rw-r--r--   0        0        0      684 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/console.py
+-rw-r--r--   0        0        0     1850 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/kaiheila.py
+-rw-r--r--   0        0        0     1723 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3940 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     1968 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/qqguild.py
+-rw-r--r--   0        0        0     3472 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/telegram.py
+-rw-r--r--   0        0        0       40 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/exception.py
+-rw-r--r--   0        0        0     2447 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/getter.py
+-rw-r--r--   0        0        0     2066 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/image_source.py
+-rw-r--r--   0        0        0      324 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/user_info.py
+-rw-r--r--   0        0        0      565 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/utils.py
+-rw-r--r--   0        0        0     1620 2023-07-27 13:03:55.169760 nonebot_plugin_userinfo-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 nonebot_plugin_userinfo-0.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_userinfo-0.0.2/LICENSE` & `nonebot_plugin_userinfo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/README.md` & `nonebot_plugin_userinfo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/__init__.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/console.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/console.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,17 @@
 
 try:
     from nonebot.adapters.console import Bot, Event
 
     @register_user_info_getter(Bot, Event)
     class Getter(UserInfoGetter[Bot, Event]):
         async def _get_info(self, user_id: str) -> Optional[UserInfo]:
-            if user_id in [self.event.user.id, self.event.user.nickname]:
-                user = self.event.user
+            user = self.event.user
+            if user_id in [user.id, user.nickname]:
                 return UserInfo(
                     user_id=user_id,
                     user_name=user.nickname,
                     user_avatar=Emoji(data=user.avatar),
                 )
 
-            if user_id in [self.bot.info.id, self.bot.info.nickname]:
-                info = self.bot.info
-                return UserInfo(
-                    user_id=user_id,
-                    user_name=info.nickname,
-                    user_avatar=Emoji(data=info.avatar),
-                )
-
 except ImportError:
     pass
```

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/kaiheila.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v11.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v12.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/qqguild.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/telegram.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/getter.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/getter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/image_source.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/image_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/utils.py` & `nonebot_plugin_userinfo-0.0.3/nonebot_plugin_userinfo/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.2/pyproject.toml` & `nonebot_plugin_userinfo-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_userinfo"
-version = "0.0.2"
+version = "0.0.3"
 description = "Nonebot2 用户信息获取插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-userinfo"
 repository = "https://github.com/noneplugin/nonebot-plugin-userinfo"
 
@@ -25,15 +25,15 @@
 nonebug = "^0.3.0"
 
 [tool.poetry.group.adapters]
 optional = true
 
 [tool.poetry.group.adapters.dependencies]
 nonebot-adapter-onebot = "^2.2.2"
-nonebot-adapter-console = "^0.3.2"
+nonebot-adapter-console = "^0.4.0"
 nonebot-adapter-qqguild = "^0.2.1"
 nonebot-adapter-kaiheila = { version = "^0.2.4", python = ">=3.9" }
 nonebot-adapter-telegram = "^0.1.0b13"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_session"]
 adapters = [
```

### Comparing `nonebot_plugin_userinfo-0.0.2/PKG-INFO` & `nonebot_plugin_userinfo-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-userinfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Nonebot2 用户信息获取插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-userinfo
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-userinfo Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-userinfo Version: 0.0.3 Summary:
 Nonebot2 ç¨æ·ä¿¡æ¯è·åæä»¶ Home-page: https://github.com/noneplugin/
 nonebot-plugin-userinfo License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: cachetools
```

