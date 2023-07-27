# Comparing `tmp/nonebot-plugin-sendmsg-by-bots-0.0.2.tar.gz` & `tmp/nonebot-plugin-sendmsg-by-bots-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.0.2.tar", last modified: Tue Jul 25 13:47:52 2023, max compression
+gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.0.3.tar", last modified: Thu Jul 27 05:47:29 2023, max compression
```

## Comparing `nonebot-plugin-sendmsg-by-bots-0.0.2.tar` & `nonebot-plugin-sendmsg-by-bots-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1831 2023-07-25 13:47:43.762863 nonebot-plugin-sendmsg-by-bots-0.0.2/README.md
--rw-r--r--   0        0        0     1098 2023-07-25 13:47:43.762863 nonebot-plugin-sendmsg-by-bots-0.0.2/nonebot_plugin_sendmsg_by_bots/__init__.py
--rw-r--r--   0        0        0      336 2023-07-25 13:47:43.762863 nonebot-plugin-sendmsg-by-bots-0.0.2/nonebot_plugin_sendmsg_by_bots/config.py
--rw-r--r--   0        0        0     2520 2023-07-25 13:47:43.762863 nonebot-plugin-sendmsg-by-bots-0.0.2/nonebot_plugin_sendmsg_by_bots/tools.py
--rw-r--r--   0        0        0      575 2023-07-25 13:47:43.762863 nonebot-plugin-sendmsg-by-bots-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2212 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1831 2023-07-27 05:47:21.706233 nonebot-plugin-sendmsg-by-bots-0.0.3/README.md
+-rw-r--r--   0        0        0     1098 2023-07-27 05:47:21.710234 nonebot-plugin-sendmsg-by-bots-0.0.3/nonebot_plugin_sendmsg_by_bots/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-27 05:47:21.710234 nonebot-plugin-sendmsg-by-bots-0.0.3/nonebot_plugin_sendmsg_by_bots/config.py
+-rw-r--r--   0        0        0     2540 2023-07-27 05:47:21.710234 nonebot-plugin-sendmsg-by-bots-0.0.3/nonebot_plugin_sendmsg_by_bots/tools.py
+-rw-r--r--   0        0        0      575 2023-07-27 05:47:21.710234 nonebot-plugin-sendmsg-by-bots-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2212 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.0.3/PKG-INFO
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.0.2/README.md` & `nonebot-plugin-sendmsg-by-bots-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sendmsg-by-bots-0.0.2/nonebot_plugin_sendmsg_by_bots/__init__.py` & `nonebot-plugin-sendmsg-by-bots-0.0.3/nonebot_plugin_sendmsg_by_bots/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sendmsg-by-bots-0.0.2/nonebot_plugin_sendmsg_by_bots/tools.py` & `nonebot-plugin-sendmsg-by-bots-0.0.3/nonebot_plugin_sendmsg_by_bots/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,47 +17,47 @@
 
 async def send_group_forward_msg_by_bots(group_id:int,node_msg:list) -> bool:
     '''group_id：尝试发送到的群号\n
     msg：尝试发送的node列表\n
     不在bot群列表的群不会尝试发送'''
     bots = nonebot.get_adapter(Adapter).bots
     for bot in bots:
-        if await is_in_group(bots[bot],group_id):
+        if await is_in_group(bots[bot],int(group_id)):
             await bots[bot].send_group_forward_msg(group_id=int(group_id), messages=node_msg)
             return True
         return False
         
 async def send_private_forward_msg_by_bots(user_id:int,node_msg:list) -> bool:
     '''user_id：尝试发送到的好友qq号\n
     msg：尝试发送的node列表\n
     不在bot好友列表的qq不会尝试发送'''
     bots = nonebot.get_adapter(Adapter).bots
     for bot in bots:
-        if await is_in_friend(bots[bot],user_id):
+        if await is_in_friend(bots[bot],int(user_id)):
             await bots[bot].send_private_forward_msg(user_id=int(user_id), messages=node_msg)
             return True
         return False
             
 async def send_group_msg_by_bots(group_id:int,msg:Message|MessageSegment|str) -> bool:
     '''group_id：尝试发送到的群号\n
     msg：尝试发送的消息\n
     不在bot群列表的群不会尝试发送'''
     bots = nonebot.get_adapter(Adapter).bots
     for bot in bots:
-        if await is_in_group(bots[bot],group_id):
+        if await is_in_group(bots[bot],int(group_id)):
             await bots[bot].send_group_msg(group_id=int(group_id),message=msg)
             return True
         return False
 
 async def send_private_msg_by_bots(user_id:int,msg:Message|MessageSegment|str) -> bool:
     '''user_id：尝试发送到的好友qq号\n
     msg：尝试发送的消息\n
     不在bot好友列表的qq不会尝试发送'''
     bots = nonebot.get_adapter(Adapter).bots
     for bot in bots:
-        if await is_in_friend(bots[bot],user_id):
+        if await is_in_friend(bots[bot],int(user_id)):
             await bots[bot].send_private_msg(user_id=int(user_id),message=msg)
             return True
         return False
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.0.2/pyproject.toml` & `nonebot-plugin-sendmsg-by-bots-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-sendmsg-by-bots"
-version = "0.0.2"
+version = "0.0.3"
 description = "a send msg tools"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.0.2/PKG-INFO` & `nonebot-plugin-sendmsg-by-bots-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sendmsg-by-bots
-Version: 0.0.2
+Version: 0.0.3
 Summary: a send msg tools
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-sendmsg-by-bots
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-sendmsg-by-bots
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sendmsg-by-bots Version: 0.0.2
+Metadata-Version: 2.1 Name: nonebot-plugin-sendmsg-by-bots Version: 0.0.3
 Summary: a send msg tools License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-sendmsg-by-bots Project-URL: Repository, https://
 github.com/nek0us/nonebot-plugin-sendmsg-by-bots Description-Content-Type:
 text/markdown
                             x [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

