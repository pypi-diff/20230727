# Comparing `tmp/nonebot_plugin_nonememe-0.1.0.tar.gz` & `tmp/nonebot_plugin_nonememe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nonememe-0.1.0.tar", last modified: Thu Jul 27 07:48:42 2023, max compression
+gzip compressed data, was "nonebot_plugin_nonememe-0.1.1.tar", last modified: Thu Jul 27 07:55:29 2023, max compression
```

## Comparing `nonebot_plugin_nonememe-0.1.0.tar` & `nonebot_plugin_nonememe-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-27 07:48:26.127584 nonebot_plugin_nonememe-0.1.0/LICENSE
--rw-r--r--   0        0        0     3548 2023-07-27 07:48:26.127584 nonebot_plugin_nonememe-0.1.0/README.md
--rw-r--r--   0        0        0      853 2023-07-27 07:48:26.127584 nonebot_plugin_nonememe-0.1.0/nonebot_plugin_nonememe/__init__.py
--rw-r--r--   0        0        0     2277 2023-07-27 07:48:26.127584 nonebot_plugin_nonememe-0.1.0/nonebot_plugin_nonememe/__main__.py
--rw-r--r--   0        0        0      381 2023-07-27 07:48:26.127584 nonebot_plugin_nonememe-0.1.0/nonebot_plugin_nonememe/config.py
--rw-r--r--   0        0        0     1864 2023-07-27 07:48:26.127584 nonebot_plugin_nonememe-0.1.0/nonebot_plugin_nonememe/data_source.py
--rw-r--r--   0        0        0      635 2023-07-27 07:48:42.583697 nonebot_plugin_nonememe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3532 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/README.md
+-rw-r--r--   0        0        0      853 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/__init__.py
+-rw-r--r--   0        0        0     2287 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/__main__.py
+-rw-r--r--   0        0        0      381 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/config.py
+-rw-r--r--   0        0        0     1864 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/data_source.py
+-rw-r--r--   0        0        0      635 2023-07-27 07:55:29.951166 nonebot_plugin_nonememe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_nonememe-0.1.0/LICENSE` & `nonebot_plugin_nonememe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.1.0/README.md` & `nonebot_plugin_nonememe-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -141,8 +141,10 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.1.1
+
+- 发送梗图会回复指令消息
```

#### html2text {}

```diff
@@ -24,9 +24,9 @@
 (https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [NoneMeme](https://nonememe.icu/) - æ¢å¾æ¥æº ##
 ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 -
+åéæ¢å¾ä¼åå¤æä»¤æ¶æ¯
```

### Comparing `nonebot_plugin_nonememe-0.1.0/nonebot_plugin_nonememe/__main__.py` & `nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 async def finish_with_meme(meme_item: MemeItem) -> NoReturn:
     image_bytes = await fetch_meme(meme_item.path)
     await MessageFactory(
         [
             Text(f"# {meme_item.name}"),
             Image(image_bytes),
         ],
-    ).finish()
+    ).finish(reply=True)
 
 
 cmd_meme = on_command("nonememe", aliases={"nb草图", "nb梗图"})
 
 
 @cmd_meme.handle()
 async def _(matcher: Matcher, state: T_State, arg_msg: Message = CommandArg()):
```

### Comparing `nonebot_plugin_nonememe-0.1.0/nonebot_plugin_nonememe/data_source.py` & `nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.1.0/pyproject.toml` & `nonebot_plugin_nonememe-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-nonememe"
-version = "0.1.0"
+version = "0.1.1"
 description = "The daily life of the NoneBot group members"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "pydantic>=1.10.4,<2",
```

### Comparing `nonebot_plugin_nonememe-0.1.0/PKG-INFO` & `nonebot_plugin_nonememe-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nonememe
-Version: 0.1.0
+Version: 0.1.1
 Summary: The daily life of the NoneBot group members
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
@@ -157,8 +157,10 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.1.1
+
+- 发送梗图会回复指令消息
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.1.0 Summary: The
+Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.1.1 Summary: The
 daily life of the NoneBot group members Home-page: https://github.com/lgc-
 NB2Dev/nonebot-plugin-nonememe Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-nonememe Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: pydantic<2,>=1.10.4 Requires-Dist: nonebot-
 plugin-send-anything-anywhere>=0.2.7 Requires-Dist: httpx>=0.24.1 Requires-
 Dist: json5>=0.9.14 Description-Content-Type: text/markdown
@@ -32,9 +32,9 @@
 (https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [NoneMeme](https://nonememe.icu/) - æ¢å¾æ¥æº ##
 ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 -
+åéæ¢å¾ä¼åå¤æä»¤æ¶æ¯
```

