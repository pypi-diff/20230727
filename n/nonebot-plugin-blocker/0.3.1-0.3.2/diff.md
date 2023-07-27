# Comparing `tmp/nonebot_plugin_blocker-0.3.1.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.1.tar", last modified: Mon Jul 24 21:46:30 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.2.tar", last modified: Thu Jul 27 16:37:11 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.1.tar` & `nonebot_plugin_blocker-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/LICENSE
--rw-r--r--   0        0        0     2447 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/README.md
--rw-r--r--   0        0        0      381 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3578 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     2589 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2370 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     2998 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     5056 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2292 2023-07-24 21:46:13.340092 nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      664 2023-07-24 21:46:30.680556 nonebot_plugin_blocker-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2447 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/README.md
+-rw-r--r--   0        0        0      381 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3624 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     2544 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2370 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     2998 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     5056 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2292 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      640 2023-07-27 16:37:11.966692 nonebot_plugin_blocker-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.1/LICENSE` & `nonebot_plugin_blocker-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.1/README.md` & `nonebot_plugin_blocker-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,54 +14,54 @@
 from .config import BlockerList, get_reply_config
 from . import web
 
 blockerlist: BlockerList
     
 driver.server_app.mount("/blocker-webui", web.app, name="blocker-webui")
 logger.info("[Blocker]WebUI is now listening on "
-            f"<u><e>http://{driver.config.host}:{driver.config.port}/blocker-webui/</e></u>"
+            f"http://{driver.config.host}:{driver.config.port}/blocker-webui/"
 )
 
 @driver.on_startup
 async def load_blocker_on_start():
     global blockerlist
     blockerlist = BlockerList()
 
 @driver.on_shutdown
 async def save_blocker_on_shut():
     global blockerlist
     del blockerlist
     
-def msg_checker(msg: str,uid: str) -> bool|None:
+async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
+    if (event.get_plaintext().find('qq') != -1 and not event.is_tome()) or event.user_id == event.self_id:
+        return False
     try:
-        reply_config = get_reply_config().get(uid)
-        if re.match(reply_config.get("command_on")+'$', msg) is not None:
+        reply_config = get_reply_config().get(str(event.self_id))
+        if re.match(reply_config.get("command_on")+'$', event.get_plaintext()) is not None:
+            state['blocker_state'] = True
+            return True
+        elif re.match(reply_config.get("command_off")+'$', event.get_plaintext()) is not None:
+            state['blocker_state'] = False
             return True
-        elif re.match(reply_config.get("command_off")+'$', msg) is not None:
-            return False
     except (AttributeError,KeyError,TypeError):
-        if re.match('[.。]bot on\s?(|\[at:qq=\d+\])', msg) is not None:
+        if re.match('[.。]bot on\s?(|\[at:qq=\d+\])', event.get_plaintext()) is not None:
+            state['blocker_state'] = True
             return True
-        elif re.match('[.。]bot off\s?(|\[at:qq=\d+\])', msg) is not None:
-            return False
-    return None
-
-async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
-    if (event.get_plaintext().find('qq') != -1 and not event.is_tome()) or event.user_id == event.self_id:
-        return False
-    state['blocker_state'] = msg_checker(event.get_plaintext(), str(event.self_id))
-    return True if state['blocker_state'] is not None else False
+        elif re.match('[.。]bot off\s?(|\[at:qq=\d+\])', event.get_plaintext()) is not None:
+            state['blocker_state'] = False
+            return True
+    return False
     
 blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2, block=True)
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher, event: GroupMessageEvent):
-    if blockerlist.check_blocker(event.group_id, event.self_id) and msg_checker(event.get_plaintext(), str(event.self_id)) is None:
+    if blockerlist.check_blocker(event.group_id, event.self_id) and re.match('^nonebot_plugin_blocker$',matcher.plugin_name) is None:
         logger.info('[Blocker]Your Message is Blocked By Blocker.')
-        await matcher.finish()
+        matcher.handlers = None
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher, event: GroupMessageEvent, state: T_State):
     reply_config = get_reply_config().get(str(event.self_id))
     if state['blocker_state']:
         blockerlist.del_blocker(event.group_id, event.self_id)
         logger.info('[Blocker]Delete Blocker Successful.')
@@ -77,12 +77,12 @@
         logger.info('[Blocker]Add Blocker Successful.')
         try:
             msg_type = reply_config.get("reply_off_type")
             msg_data = reply_config.get("reply_off_content")
             if msg_data == "":
                 raise AttributeError
         except AttributeError:
-            await matcher.finish('在本群开启')
+            await matcher.finish('在本群关闭')
     if msg_type == "text":
         await matcher.finish(msg_data)
     else:
         await matcher.finish(MessageSegment(type=msg_type, data={"file":msg_data}))
```

### Comparing `nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/config.py` & `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,18 +65,16 @@
             self.blocklist[str(qid)].remove(gid)
         except:
             pass
         
     def check_blocker(self,gid: int, qid: int) -> bool:
         try:
             self.blocklist[str(qid)].index(gid)
+            return True
         except:
             return False
-        else:
-            return True
 
     def __del__(self):
-        with BLOCKLIST_JSON_PATH.open('w', encoding='UTF-8') as file:
-            json.dump(self.blocklist, file, ensure_ascii=False)
+        json.dump(self.blocklist, BLOCKLIST_JSON_PATH.open('w', encoding='UTF-8'), ensure_ascii=False)
             
 driver_config = get_driver().config
 config = PluginConfig.parse_obj(driver_config.dict())
```

### Comparing `nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.1/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.1/pyproject.toml` & `nonebot_plugin_blocker-0.3.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.1"
+version = "0.3.2"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
     "qqbot",
     "bot",
 ]
 dependencies = [
     "nonebot2[fastapi] >= 2.0.0",
-    "pydantic>=1.10.4",
     "nonebot-adapter-onebot>=2.1.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 file = "LICENSE"
```

### Comparing `nonebot_plugin_blocker-0.3.1/PKG-INFO` & `nonebot_plugin_blocker-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.1
+Version: 0.3.2
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
@@ -13,15 +13,14 @@
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2[fastapi]>=2.0.0
-Requires-Dist: pydantic>=1.10.4
 Requires-Dist: nonebot-adapter-onebot>=2.1.0
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.2 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -13,16 +13,16 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Requires-Dist: nonebot2
-[fastapi]>=2.0.0 Requires-Dist: pydantic>=1.10.4 Requires-Dist: nonebot-
-adapter-onebot>=2.1.0 Description-Content-Type: text/markdown
+[fastapi]>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.1.0 Description-
+Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
 æä»¶æä¾äºä¸ä¸ªç®åçWebUIæ¥è®©ä½ éç½®Botçå¼å³æä»¤ä»¥åå¯¹æä»¤ååºçåå¤ã
```

