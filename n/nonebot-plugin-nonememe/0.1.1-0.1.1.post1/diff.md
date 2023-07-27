# Comparing `tmp/nonebot_plugin_nonememe-0.1.1.tar.gz` & `tmp/nonebot_plugin_nonememe-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nonememe-0.1.1.tar", last modified: Thu Jul 27 07:55:29 2023, max compression
+gzip compressed data, was "nonebot_plugin_nonememe-0.1.1.post1.tar", last modified: Thu Jul 27 08:19:59 2023, max compression
```

## Comparing `nonebot_plugin_nonememe-0.1.1.tar` & `nonebot_plugin_nonememe-0.1.1.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/LICENSE
--rw-r--r--   0        0        0     3532 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/README.md
--rw-r--r--   0        0        0      853 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/__init__.py
--rw-r--r--   0        0        0     2287 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/__main__.py
--rw-r--r--   0        0        0      381 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/config.py
--rw-r--r--   0        0        0     1864 2023-07-27 07:55:14.102983 nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/data_source.py
--rw-r--r--   0        0        0      635 2023-07-27 07:55:29.951166 nonebot_plugin_nonememe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/LICENSE
+-rw-r--r--   0        0        0     3532 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/README.md
+-rw-r--r--   0        0        0      853 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__init__.py
+-rw-r--r--   0        0        0     2287 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__main__.py
+-rw-r--r--   0        0        0      381 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/config.py
+-rw-r--r--   0        0        0     1843 2023-07-27 08:19:44.409145 nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/data_source.py
+-rw-r--r--   0        0        0      641 2023-07-27 08:19:59.217320 nonebot_plugin_nonememe-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     4111 1970-01-01 00:00:00.000000 nonebot_plugin_nonememe-0.1.1.post1/PKG-INFO
```

### Comparing `nonebot_plugin_nonememe-0.1.1/LICENSE` & `nonebot_plugin_nonememe-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.1.1/README.md` & `nonebot_plugin_nonememe-0.1.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/__init__.py` & `nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/__main__.py` & `nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nonememe-0.1.1/nonebot_plugin_nonememe/data_source.py` & `nonebot_plugin_nonememe-0.1.1.post1/nonebot_plugin_nonememe/data_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,12 +60,11 @@
 
 async def init_meme_list():
     meme_list.clear()
     meme_list.extend(await fetch_meme_list())
     logger.opt(colors=True).success(
         f"Succeed to init meme list, Loaded <y>{len(meme_list)}</y> memes",
     )
-    print(meme_list)
 
 
 driver = get_driver()
 driver.on_startup(init_meme_list)
```

### Comparing `nonebot_plugin_nonememe-0.1.1/pyproject.toml` & `nonebot_plugin_nonememe-0.1.1.post1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-nonememe"
-version = "0.1.1"
+version = "0.1.1.post1"
 description = "The daily life of the NoneBot group members"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "pydantic>=1.10.4,<2",
```

### Comparing `nonebot_plugin_nonememe-0.1.1/PKG-INFO` & `nonebot_plugin_nonememe-0.1.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nonememe
-Version: 0.1.1
+Version: 0.1.1.post1
 Summary: The daily life of the NoneBot group members
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-nonememe
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.1.1 Summary: The
-daily life of the NoneBot group members Home-page: https://github.com/lgc-
-NB2Dev/nonebot-plugin-nonememe Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-nonememe Version: 0.1.1.post1
+Summary: The daily life of the NoneBot group members Home-page: https://
+github.com/lgc-NB2Dev/nonebot-plugin-nonememe Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-nonememe Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: pydantic<2,>=1.10.4 Requires-Dist: nonebot-
 plugin-send-anything-anywhere>=0.2.7 Requires-Dist: httpx>=0.24.1 Requires-
 Dist: json5>=0.9.14 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

