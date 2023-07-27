# Comparing `tmp/tikapi-3.1.3.tar.gz` & `tmp/tikapi-3.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikapi-3.1.3.tar", last modified: Thu Jul 27 16:25:12 2023, max compression
+gzip compressed data, was "tikapi-3.1.31.tar", last modified: Thu Jul 27 16:36:14 2023, max compression
```

## Comparing `tikapi-3.1.3.tar` & `tikapi-3.1.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 16:25:12.753670 tikapi-3.1.3/
--rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1860 2023-07-27 16:25:12.753670 tikapi-3.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.3/README.md
--rw-rw-rw-   0        0        0      121 2023-07-27 16:25:12.754671 tikapi-3.1.3/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-07-27 13:38:19.000000 tikapi-3.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:25:12.748669 tikapi-3.1.3/tikapi/
--rw-rw-rw-   0        0        0     3172 2022-12-07 20:49:56.000000 tikapi-3.1.3/tikapi/__init__.py
--rw-rw-rw-   0        0        0    86591 2023-07-27 16:23:25.000000 tikapi-3.1.3/tikapi/api.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:25:12.752670 tikapi-3.1.3/tikapi.egg-info/
--rw-rw-rw-   0        0        0     1860 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.3/tikapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 16:25:12.000000 tikapi-3.1.3/tikapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 16:36:14.932509 tikapi-3.1.31/
+-rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.31/MANIFEST.in
+-rw-rw-rw-   0        0        0     1861 2023-07-27 16:36:14.932509 tikapi-3.1.31/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.31/README.md
+-rw-rw-rw-   0        0        0      121 2023-07-27 16:36:14.933508 tikapi-3.1.31/setup.cfg
+-rw-rw-rw-   0        0        0      704 2023-07-27 16:36:05.000000 tikapi-3.1.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:36:14.927509 tikapi-3.1.31/tikapi/
+-rw-rw-rw-   0        0        0     3172 2022-12-07 20:49:56.000000 tikapi-3.1.31/tikapi/__init__.py
+-rw-rw-rw-   0        0        0    86587 2023-07-27 16:35:48.000000 tikapi-3.1.31/tikapi/api.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:36:14.932509 tikapi-3.1.31/tikapi.egg-info/
+-rw-rw-rw-   0        0        0     1861 2023-07-27 16:36:14.000000 tikapi-3.1.31/tikapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-27 16:36:14.000000 tikapi-3.1.31/tikapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:36:14.000000 tikapi-3.1.31/tikapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.31/tikapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-27 16:36:14.000000 tikapi-3.1.31/tikapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 16:36:14.000000 tikapi-3.1.31/tikapi.egg-info/top_level.txt
```

### Comparing `tikapi-3.1.3/PKG-INFO` & `tikapi-3.1.31/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.3
+Version: 3.1.31
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

### Comparing `tikapi-3.1.3/README.md` & `tikapi-3.1.31/README.md`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.3/setup.py` & `tikapi-3.1.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 INSTALL_REQUIRES = [
    'requests',
 ]
 
 setup(
     name='tikapi',
-    version='3.1.3',
+    version='3.1.31',
     description='TikAPI | TikTok Unofficial API',
     long_description_content_type="text/markdown",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     license='TikAPI',
     author='TikAPI',
     author_email='contact@tikapi.io',
     url='https://www.tikapi.io',
```

### Comparing `tikapi-3.1.3/tikapi/__init__.py` & `tikapi-3.1.31/tikapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.3/tikapi/api.py` & `tikapi-3.1.31/tikapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,18 +519,18 @@
 			'''
 			
 			return wrap({"path":"/public/related_posts","help":"Get related posts","comment":"<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","params":{"video_id":{"help":"The video ID from which to get related posts. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"}},"$other":{"openapi":{"hideParams":["session_id"],"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "Public.relatedPosts")(video_id=video_id, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
 		def playlists(cls, secUid: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
-				Get an user playlists 
+				Get a user's playlists 
 			'''
 			count = None if count is cls.playlists.__defaults__[1] else count
-			return wrap({"path":"/public/playlists","help":"Get an user playlists","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"],"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "Public.playlists")(secUid=secUid, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
+			return wrap({"path":"/public/playlists","help":"Get a user's playlists","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"],"fields":{"x-new":True}}},"method":"GET"}, cls.__get_options__(), "Public.playlists")(secUid=secUid, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
 		def playlistItems(cls, playlist_id = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a playlist items 
 			'''
 			count = None if count is cls.playlistItems.__defaults__[1] else count
@@ -1055,26 +1055,26 @@
 			'''
 			count = None if count is cls.followers.__defaults__[1] else count
 			return wrap({"help":"Get followers list","comment":"Get current user followers list (or a friends by specifying the secUid).","path":"/user/followers","params":{"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"nextCursor":{"type":"string","help":"A iteration parameter returned in each response, should be included in the next requests to get the next items."}},"$other":{"openapi":{"fields":{"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["view_followers"]}]}}},"method":"GET"}, cls.__get_options__(), "User.followers")(secUid=secUid, count=count, nextCursor=nextCursor, **otherParams)
 	
 		@classmethod
 		def follow(cls, username: str = None, secUid: str = None, user_id: str = None, **otherParams) -> APIResponse:
 			'''
-				Follow an user 
+				Follow a user 
 			'''
 			
-			return wrap({"help":"Follow an user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/follow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"hide":True,"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.follow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
+			return wrap({"help":"Follow a user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/follow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"hide":True,"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.follow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
 	
 		@classmethod
 		def unfollow(cls, username: str = None, secUid: str = None, user_id: str = None, **otherParams) -> APIResponse:
 			'''
-				Unfollows an user 
+				Unfollow a user 
 			'''
 			
-			return wrap({"help":"Unfollows an user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/unfollow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"hide":True,"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.unfollow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
+			return wrap({"help":"Unfollow a user","comment":"*This endpoint is only available to trusted customers. \n<a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-can-i-get-access-to-special-endpoints'> Learn more about special endpoints</a>*\n\n<br>This endpoint is deprecated and might not work as excpeted.","path":"/user/unfollow","method":"POST","enctype":"json","params":{"username":{"help":"The TikTok user username","validate":"^([a-zA-Z0-9_.]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","required":True,"example":"lilyachty"},"secUid":{"validate":"^(.*?){30,}$","help":"The TikTok user secUid. You can get this from the <a href='#tag/Public/operation/public.check'>Get profile information</a> endpoint using the username.","type":"string","example":"MS4wLjABAAAAsHntXC3s0AvxcecggxsoVa4eAiT8OVafVZ4OQXxy-9htpnUi0sOYSr0kGGD1Loud","required":True},"user_id":{"help":"The TikTok user ID","type":"string","validate":"^[0-9]+$","required":True,"example":"6569595380449902597"}},"$other":{"openapi":{"hide":True,"fields":{"deprecated":True,"tags":["Followers"],"security":[{"apiKey":[],"accountKey":["follow_actions"]}]}}}}, cls.__get_options__(), "User.unfollow")(username=username, secUid=secUid, user_id=user_id, **otherParams)
 	
 		posts = Rests.UserPosts
 		@classmethod
 		def conversations(cls, nextCursor: int = None, **otherParams) -> APIResponse:
 			'''
 				Get user conversations 
 			'''
```

### Comparing `tikapi-3.1.3/tikapi.egg-info/PKG-INFO` & `tikapi-3.1.31/tikapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.3
+Version: 3.1.31
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

